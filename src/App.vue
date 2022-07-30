<template>
<template v-if="page === 'home'">
  <Artesana />
</template>
<template v-else-if="page === 'historias'">
  <ArtesanaHistorias />
</template>
</template>

<script setup>
import Artesana from './components/Artesana.vue';
import ArtesanaHistorias from './components/ArtesanaHistorias.vue';

import { onBeforeUnmount, onMounted, provide, ref } from 'vue'

const page = ref('home')

const scrollPosition = ref(0)
const scrollLocked = ref(false)

provide('page', page)
provide('page/@change', newPage => {
  page.value = newPage
})
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