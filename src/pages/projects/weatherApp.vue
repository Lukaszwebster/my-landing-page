<script setup>
const projectOverviewItems = [
  {
    title: 'Aplikacja pogodowa.',
    subtitle: 'Projekt w ramach nauki',
    description: 'Projekt aplikacji pogodowej robiony w ramach nauki wykorzystywania API.',
    imgUrl: '/weatherApp.png',
    href: '',
    skills: ['html', 'tailwindCSS', 'vue'],
    details: 'W projekcie uczyłem się pobierania danych z API. Pierwszą rzeczą jaką musiałem zrobić to znależć odpowiednie darmowe dane pogodowe. Aplikacja pokazuje aktualną pogodę w wybranym przez użytkownika mieście.',
    imgStyle: 'max-h-[40rem] md:mr-[10rem]',
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
