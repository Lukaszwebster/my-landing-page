<script setup>
const projectOverviewItems = [
  {
    title: 'Clipboard Landing Page.',
    subtitle: 'Landing page z Frontend Mentor.',
    description: 'Projekt z Frontend Mentor, w którym uczyłem się podstaw css. Największym wyzwaniem była dla mnie responsywność.',
    imgUrl: '/clipboard.jpeg',
    href: 'https://lukaszwebster.github.io/clipboard-landing-page-master/',
    skills: ['html', 'tailwindCSS', 'js'],
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
