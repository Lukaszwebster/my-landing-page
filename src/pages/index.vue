<script setup lang="ts">
const projects = [
  {
    title: 'Wycena.AI',
    subtitle: 'Wycena nieruchomowści. Pierwszy komercyjny projekt, w którym, brałem udział jako junior.',
    imgSrc: '/wycena-ai.png',
    imgUrl: 'https://wycena.ai',
    to: '/projects/wycenaai',
    buttonText: 'Moje doświadczenie',
  },
  {
    title: 'MediDent',
    subtitle: 'Mój projekt strony dla zaprzyjaźnionego gabinetu stomatologicznego. Od projektu, przez zdjęcia aż do kodu wykonany przeze mnie. Projekt nauczył mnie wielu rzeczy.',
    imgSrc: '/MediDentImg.png',
    imgUrl: 'https://medidentpulawy.pl',
    to: '/projects/mediDent',
    buttonText: 'Przeczytaj więcej',
  },
  {
    title: 'Social Seal',
    subtitle: 'Landing Page wykonany dla jednej z firm do których aplikowałem.',
    imgSrc: '/socialSeal.png',
    imgUrl: 'https://splendorous-phoenix-798e6b.netlify.app/',
    buttonText: 'Przeczytaj więcej',
    to: '/projects/socialSeal',
  },
  {
    title: 'URL Shortening. Frontend Mentor.',
    subtitle: 'Jeden z moich pierwszych projektów. Pomysł z Frontend Mentora. Jest to prosty landing page, którego zadaniem jest skracać linki. Wykorzystałem w nim tailwind CSS.',
    imgSrc: '/shortly.jpeg',
    imgUrl: 'https://lukaszwebster.github.io/Shortly-URL/',
    buttonText: 'O projekcie',
    to: '/projects/urlShortening',
  },
  {
    title: 'Clipboard landing page. Frontend Mentor',
    subtitle: 'Kolejny projekt ze strony frontend Mentor, który robiłem w ramach nauki.',
    imgSrc: '/clipboard.jpeg',
    imgUrl: 'https://lukaszwebster.github.io/clipboard-landing-page-master/',
    buttonText: 'O projekcie',
    to: '/projects/landingPage',
  },
  {
    title: 'Weather app',
    subtitle: ' Aplikacja pogodowa pokazująca aktualne dane pogodowe miast. W krótce będzie rozbudowywana.',
    imgSrc: '/weatherApp.png',
    imgUrl: '',
    to: '/projects/weatherApp',
    buttonText: 'O projekcie',
    class: 'max-w-[20rem]',
  },
]
</script>

<template>
  <div>
    <TheHeader />
    <TheSkills data-aos="fade-zoom-in" data-aos-offset="200" data-aos-easing="ease-in-sine" data-aos-duration="800" />
    <div class="mx-auto mt-20 max-w-[90rem] items-center px-4 font-roboto md:mt-30 lg:px-[80px]" data-aos="fade-zoom-in" data-aos-offset="200" data-aos-easing="ease-in-sine" data-aos-duration="800">
      <h2 class="text-center text-[1.5rem] md:text-left">
        Moje projekty
      </h2>
      <h2 class="mt-4 text-center leading-loose text-gray-500 lg:max-w-[550px] md:max-w-400px md:text-left dark:text-gray-400">
        Oto kilka moich projektów, które wiele mnie nauczyły oraz ukierunkowały na dalszy rozwój. Skupiam się w nich mocno na responsywności oraz przejrzystości kodu. Znajdują się tutaj zarówno strony komercyjne jak i te, które wykonałem w ramach nauki.
      </h2>
    </div>
    <AppProject v-for="(item, index) in projects" :key="index" v-bind="item" />
  </div>
</template>
