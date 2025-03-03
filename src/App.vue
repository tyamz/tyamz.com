<script setup lang="ts">
import { ref, computed, type ComponentCustomElementInterface } from 'vue'
import HomePage from './components/HomePage.vue'
import MenuComponent from './components/MenuComponent.vue'
import AboutPage from './components/AboutPage.vue'
const routes: Record<string, ComponentCustomElementInterface> = {
  '/': HomePage,
  '/about': AboutPage,
}

const currentPath = ref(window.location.hash)

window.addEventListener('hashchange', () => {
  currentPath.value = window.location.hash
})

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || '/']
})
</script>

<template>
  <component :is="currentView" />
  <MenuComponent />
</template>

<style scoped></style>
