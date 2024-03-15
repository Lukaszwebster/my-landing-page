<script setup>
const skills = [
  {
    id: 1,
    name: 'HTML',
  },
  {
    id: 2,
    name: 'CSS',
  },
  {
    id: 3,
    name: 'JavaScript',
  },
  {
    id: 4,
    name: 'Tailwind CSS',
  },
  {
    id: 5,
    name: 'Windi CSS',
  },
  {
    id: 6,
    name: 'Uno CSS',
  },
  {
    id: 7,
    name: 'Vue',
  },
  {
    id: 8,
    name: 'Vite',
  },
  {
    id: 9,
    name: 'RWD',
  },
  {
    id: 10,
    name: 'GIT',
  },
  {
    id: 11,
    name: 'Nuxt',
  },
  {
    id: 12,
    name: 'SASS',
  },
  {
    id: 13,
    name: 'SCSS',
  },
  {
    id: 14,
    name: 'Adobe XD',
  },
  {
    id: 15,
    name: 'Figma',
  },
  {
    id: 16,
    name: 'Adobe Photoshop',
  },
  {
    id: 17,
    name: 'Adobe Lightroom',
  },
]
</script>

<template>
  <div class="mx-auto mt-30 max-w-[90rem] px-4 font-roboto lg:px-[80px]">
    <h2 class="text-[1.5rem]">
      Technologie z których korzystam
    </h2>
    <div class="justify-between md:flex">
      <h2 class="mt-4 leading-loose text-gray-500 lg:max-w-[550px] md:max-w-300px dark:text-gray-400">
        O kiedy zajmuję się frontendem,  staram się poznawać jak najwięcej nowych technologii. Uważam że tylko ciągłą nauką można nadążyć za dynamicznie rozwijającą się branżą IT.
        Dzięki temu jestem otwarty na kolejne wyzwania i chcę aby mój "frontendowy warsztat pracy" był jak najbardziej obszerny. Widzę również dużo sensu w nabywaniu umiejętności dodatkowych takich jak obsługa popularnych programów od Adobe. Pomaga to w rozwijaniu własnych projektów jak również zleceń mniejszych klientów.
      </h2>
      <div class="mt-10 md:mt-0 lg:max-w-400px md:max-w-300px md:text-right">
        <AppSkillsItems v-for="item in skills" :key="item.id" v-bind="item" />
      </div>
    </div>
  </div>
</template>
