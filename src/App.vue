<template>
  <Artesana />
</template>

<script setup>
import Artesana from './components/Artesana.vue';

import { onBeforeUnmount, onMounted, provide, ref } from 'vue'

const scrollPosition = ref(0)
const scrollLocked = ref(false)

provide('scroll', scrollPosition)

function updateScroll() {
  if (!scrollLocked.value) {
    window.requestAnimationFrame(() => {
      scrollPosition.value = window.scrollY
      scrollLocked.value = false
    })

  }
  scrollLocked.value = true
}

onMounted(() => {
  window.addEventListener('scroll', updateScroll)
})

onBeforeUnmount(() => {
  window.removeEventListener('scroll', updateScroll)
})
</script>