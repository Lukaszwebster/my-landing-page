<script setup>
const projectOverviewItems = [
  {
    title: 'Social Seal landing page',
    subtitle: 'Landing page, który wykonałem w ramach rekrutacji.',
    description: '',
    imgUrl: '/socialSeal.png',
    href: 'https://splendorous-phoenix-798e6b.netlify.app/',
    skills: ['vue', 'unocss'],
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
