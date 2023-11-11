<script setup>
const projectOverviewItems = [
  {
    title: 'MediDent.',
    subtitle: 'Gabinet stomatologiczny.',
    description: 'MediDent to zaprzyjaźniony gabinet stomatologiczny. Gdy tylko dowiedziałem się, że firmie potrzebna jest strona internetowa postanowiłem nie odpłatnie ją wykonać. Praca nad projektem była ciekawym doświadczeniem.',
    imgUrl: '/MediDentImg.png',
    href: 'https://medidentpulawy.pl/',
    skills: ['vue', 'vite', 'UnoCss', 'vue router'],
    details: 'Przy pracy ze strona MediDent napotkałem wiele wyzwań ponieważ projekt musiał być stworzony od początku do końca. oznaczało to, że do mnie należało wybranie technologii, wymyślenie wyglądu strony, wykonanie zdjęć w firmie oraz teksty. Uświadomiło mi to jak trudne jest wykonanie wszystkiego samodzielnie i jak bardzo w innych projektach liczą się role poszczególnych członków teamu.',
  },
]
</script>

<template>
  <div>
    <AppProjectOverview v-for="(item, index) in projectOverviewItems" :key="index" v-bind="item" />
  </div>
</template>
