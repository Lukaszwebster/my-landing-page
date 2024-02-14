<script setup>
const projectOverviewItems = [
  {
    title: 'Social Seal landing page',
    subtitle: 'Landing page, który wykonałem w ramach rekrutacji dla jednej z firm. Początkowo miał być wykonany tylko w celu wysłania go do potencjalnego pracodawcy. W procesie tworzenia projektu zauważyłem jednak, że nauczył mnie wielu nowych rzeczy i postanowiłem umieścić go tutaj.',
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
