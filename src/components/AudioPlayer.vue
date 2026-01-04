<script setup>
import { ref, watch, onMounted } from 'vue'

const props = defineProps({
  src: { type: String, required: true },
  number: { type: Number, default: 1 }
})

const audio = ref(null)

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

</script>

<template>
    <div>
        Audio {{ number }}
        <button @click="togglePlay">Play/Pause</button>
        <audio ref="audio" :src="src"></audio>
    </div>
</template>