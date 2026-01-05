<script setup>
import AudioPlayer from './components/AudioPlayer.vue'
</script>

<template>
  <h1>Greek Audio Lessons</h1>
  
  <h2>Introduction</h2>
  <AudioPlayer src="../assets/01-IntroductoryLesson.mp3" number="1" />

  <h2>Lesson 1</h2>
  
  <span>Γειά σας <AudioPlayer src="../assets/02-Lesson1-1.mp3" number="2" /></span>
  <span>Πώς σας λένε; <AudioPlayer src="../assets/03-Lesson1-2.mp3" number="3" /></span>
  <span>Γειά σου <AudioPlayer src="../assets/04-Lesson1-3.mp3" number="4" /></span>
  <span>Πώς σε λένε; <AudioPlayer src="../assets/05-Lesson1-4.mp3" number="5" /></span>
  <span>Από πού είστε; <AudioPlayer src="../assets/06-Lesson1-5.mp3" number="6" /></span>
  <span>Από πού είσαι; <AudioPlayer src="../assets/07-Lesson1-6.mp3" number="7" /></span>
</template>

<style scoped></style>
