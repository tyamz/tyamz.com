<script setup lang="ts">
import { ref } from 'vue'
const showMenu = ref(false)
</script>

<template>
  <div class="menu" v-if="showMenu">
    <ul>
      <li><a href="#/" @click="showMenu = false">Home</a></li>
      <li><a href="#/about" @click="showMenu = false">About Me</a></li>
      <li><a href="https://github.com/tyamz" target="_blank">GitHub</a></li>
      <li><a href="https://linkedin.com/in/thomas-yamakaitis" target="_blank">LinkedIn</a></li>
      <li><a href="/ThomasYamakaitis-Resume.pdf" target="_blank">Resume</a></li>
    </ul>
  </div>
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
</style>
