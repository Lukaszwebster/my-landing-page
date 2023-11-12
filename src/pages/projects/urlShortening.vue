<script setup>
const projectOverviewItems = [
  {
    title: 'URL Shortening.',
    subtitle: 'Skracanie linków z Frontend Mentor.',
    description: ' Jest to jeden z pierwszych moich projektów, który wykonywałem w ramach nauki z serwisem Frontend Mentor.',
    imgUrl: '/shortly.jpeg',
    href: 'https://lukaszwebster.github.io/Shortly-URL/',
    skills: ['html', 'tailwindCSS', 'java script'],
    details: 'Był to pierwszy projekt w, którym musiałem pobrać dane z API.',
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
