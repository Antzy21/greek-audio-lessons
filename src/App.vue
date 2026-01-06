<script setup>
import AudioPlayer from './components/AudioPlayer.vue'
</script>

<template>
  <h1>Greek Audio Lessons</h1>
  
  <h2>Introduction</h2>

  <div>
    <span>Letters and Sounds <AudioPlayer src="../assets/01-IntroductoryLesson.mp3" buttonText="1" /></span>
  </div>

  <h2>Lesson 1</h2>
  
  <div>
    <span>Γειά σας <AudioPlayer src="../assets/02-Lesson1-1.mp3" buttonText="2" /></span>
    <span>Πώς σας λένε; <AudioPlayer src="../assets/03-Lesson1-2.mp3" buttonText="3" /></span>
    <span>Γειά σου <AudioPlayer src="../assets/04-Lesson1-3.mp3" buttonText="4" /></span>
    <span>Πώς σε λένε; <AudioPlayer src="../assets/05-Lesson1-4.mp3" buttonText="5" /></span>
    <span>Από πού είστε; <AudioPlayer src="../assets/06-Lesson1-5.mp3" buttonText="6" /></span>
    <span>Από πού είσαι; <AudioPlayer src="../assets/07-Lesson1-6.mp3" buttonText="7" /></span>
  </div>

  <h2>Lesson 2</h2>

  <div>
    <span>Καλημέρα σας. Τι κάνετε; <AudioPlayer src="../assets/08-Lesson2-1.mp3" buttonText="8" /></span>
    <span>Γειά σου. Τι κάνεις; <AudioPlayer src="../assets/09-Lesson2-2.mp3" buttonText="9" /></span>
    <span>Η κυρία Γιαρδέλ. Ο κύριος Μαρατός. <AudioPlayer src="../assets/10-Lesson2-3.mp3" buttonText="10" /></span>
    <span>Ο Στέφαν. Η Μόνικα. <AudioPlayer src="../assets/11-Lesson2-4.mp3" buttonText="11" /></span>
  </div>

  <div>
    <span>Exercise 6 <AudioPlayer src="../assets/12-Lesson2-5.mp3" buttonText="12" /></span>
  </div>

  <h2>Lesson 3</h2>

  <div>
    <span>Η Μόνικ δουλεύει στην Ελλάδα <AudioPlayer src="../assets/13-Lesson3-1.mp3" buttonText="13" /></span>
    <span>Είμαι απ' τη Ρωσία, απ' τη Μόσχα <AudioPlayer src="../assets/14-Lesson3-2.mp3" buttonText="14" /></span>
    <span>Πού μένετε; <AudioPlayer src="../assets/15-Lesson3-3.mp3" buttonText="15" /></span>
  </div>

  <div>
    <span>Exercise 12 <AudioPlayer src="../assets/16-Lesson3-4.mp3" buttonText="16" /></span>
  </div>

  <h2>Lesson 4</h2>

  <div>
    <span>Πώς λέγεστε, παρακαλώ <AudioPlayer src="../assets/17-Lesson4-1.mp3" buttonText="17" /></span>
    <span>Το τηλέφωνό μου είναι 210 9519263 <AudioPlayer src="../assets/18-Lesson4-2.mp3" buttonText="18" /></span>
    <span>Τι δουλειά κάνετε; <AudioPlayer src="../assets/19-Lesson4-3.mp3" buttonText="19" /></span>
    <span>Τι δουλειά κάνεις; <AudioPlayer src="../assets/20-Lesson4-4.mp3" buttonText="20" /></span>
  </div>

  <div>
    <span>Exercise 11 <AudioPlayer src="../assets/21-Lesson4-5.mp3" buttonText="21" /></span>
  </div>

  <h2>Lesson 5</h2>

  <div>
    <span>Μιλάς ελληνικά; <AudioPlayer src="../assets/22-Lesson5-1.mp3" buttonText="22" /></span>
  </div>

  <div>
    <span>Exercise 9 <AudioPlayer src="../assets/23-Lesson5-2.mp3" buttonText="23" /></span>
  </div>

  <h2>Lesson 6</h2>

  <div>
    <span>Από την Ισπανία στην Ελλάδα <AudioPlayer src="../assets/24-Lesson6.mp3" buttonText="24" /></span>
  </div>

  <footer>
    <hr/>
    Audio belongs to <a href="https://deltos.gr" target="_blank">deltos.gr</a> <br/>
    Developed by Antzy21
  </footer>
  
</template>

<style scoped></style>
