<script setup lang="ts">
import { ref } from 'vue'
const showMenu = ref(false)
</script>

<template>
  <Transition name="slide-fade">
    <div v-if="showMenu" class="menu">
      <ul>
        <li><a href="#/" @click="showMenu = false">Home</a></li>
        <li><a href="#/about" @click="showMenu = false">About Me</a></li>
        <li><a href="https://github.com/tyamz" target="_blank">GitHub</a></li>
        <li><a href="https://linkedin.com/in/thomas-yamakaitis" target="_blank">LinkedIn</a></li>
        <li><a href="/ThomasYamakaitis-Resume.pdf" target="_blank">Resume</a></li>
      </ul>
    </div>
  </Transition>
  <footer>
    <button @click="showMenu = !showMenu" class="menu-btn">^</button>
  </footer>
</template>

<style scoped>
.menu {
  position: fixed;
  display: flex;
  justify-content: center;
  height: 100%;
  width: 100%;
  background: #333;
  opacity: 95%;
}

ul li {
  font-size: 2rem;
  margin: 1rem 0;
}

/*
  Enter and leave animations can use different
  durations and timing functions.
*/
.slide-fade-enter-active {
  transition: all 0.25s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.25s cubic-bezier(1, 0.5, 0.8, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateY(100%);
  opacity: 0;
}
</style>
