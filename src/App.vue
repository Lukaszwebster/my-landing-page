<script setup lang="ts">
import AOS from 'aos'
import 'aos/dist/aos.css'

AOS.init()
// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be rendered correctly in the html results with vite-ssg
useHead({
  title: 'Landing page',
  meta: [
    { name: 'description', content: 'Landing Page' },
    {
      name: 'theme-color',
      content: () => isDark.value ? '#00aba9' : '#ffffff',
    },
  ],

})
</script>

<template>
  <RouterView />
</template>
