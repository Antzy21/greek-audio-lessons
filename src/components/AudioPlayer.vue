<script setup>
import { ref, watch, onMounted, onUnmounted } from 'vue'

const props = defineProps({
  src: { type: String, required: true },
  buttonText: { type: String, default: "" }
})

const audio = ref(null)
const isPlaying = ref(false)

function play() {
    audio.value?.play().catch(() => {})
}

function pause() {
    audio.value?.pause()
}

function togglePlay() {
    if (audio.value?.paused) {
        play()
    } else {
        pause()
    }
}

watch(() => props.src, (newSrc) => {
  if (audio.value) {
    audio.value.src = newSrc || ''
    audio.value.load()
  }
})

onMounted(() => {
  if (!audio.value) return
  // keep play/pause/ended in sync with state
  const onPlay = () => { isPlaying.value = true }
  const onPause = () => { isPlaying.value = false }
  const onEnded = () => { isPlaying.value = false }
  audio.value.addEventListener('play', onPlay)
  audio.value.addEventListener('pause', onPause)
  audio.value.addEventListener('ended', onEnded)
  // store listeners for cleanup
  audio._listeners = { onPlay, onPause, onEnded }
})

onUnmounted(() => {
  if (!audio.value || !audio._listeners) return
  const { onPlay, onPause, onEnded } = audio._listeners
  audio.value.removeEventListener('play', onPlay)
  audio.value.removeEventListener('pause', onPause)
  audio.value.removeEventListener('ended', onEnded)
  delete audio._listeners
})

</script>

<template>
  <button class="play-btn" :class="{ playing: isPlaying }" @click="togglePlay" :aria-pressed="isPlaying" aria-label="Play or pause audio">
    {{ buttonText }}
  </button>
  <audio ref="audio" :src="src"></audio>
</template>