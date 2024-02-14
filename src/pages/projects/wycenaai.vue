<script setup>
const projectOverviewItems = [
  {
    title: 'Wycena.AI',
    subtitle: 'Wycena nieruchomości',
    description: 'Był to mój pierwszy projekt komercyjny, w którym pracowałem jako junior. Projekt ten składa się z dwóch części. Landing page z podstronami oraz aplikacji do wyceny nieruchomości dostępnej po zalogowaniu.',
    imgUrl: '/wycena-ai.png',
    href: 'https://wycena.ai',
    skills: ['vue', 'vite', 'nuxt', 'tailwind'],
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
