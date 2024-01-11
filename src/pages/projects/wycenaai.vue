<script setup>
const projectOverviewItems = [
  {
    title: 'Wycena.AI',
    subtitle: 'Wycena nieruchomości',
    description: 'Był to mój pierwszy projekt komercyjny',
    imgUrl: '/wycena-ai.png',
    href: 'https://wycena.ai',
    skills: [],
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
