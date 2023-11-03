<script setup>
const techItems = ['html', 'css', 'js']
</script>

<template>
  <div class="mx-4 mt-12 font-roboto 2xl:mx-[300px] lg:mx-[80px]">
    <div class="max-w-[40rem]">
      <h1 class="text-[1.8rem] font-500">
        Clipboard Landing Page.
      </h1>
      <h2 class="text-gray">
        Landing page z Frontend Mentor
      </h2>
      <p class="mt-12 text-gray">
        Projekt z Frontend Mentor, w którym uczyłem się podstaw css. Największym wyzwaniem była dla mnie responsywność.
      </p>
    </div>
    <div class="mt-[4rem] w-full flex flex-col justify-between md:flex-row">
      <div>
        <h2 class="text-gray">
          Technologie w projekcie
        </h2>
        <div class="mt-[2rem] flex flex-col gap-1">
          <ul v-for="(item, index) in techItems" :key="index">
            <li class="w-min rounded-4px bg-#fafafa px-2 py-1 hover:bg-gray dark:text-black">
              {{ item }}
            </li>
          </ul>
        </div>
        <div class="mt-[2rem]">
          <a class="underline" href="https://lukaszwebster.github.io/clipboard-landing-page-master/">Obejrzyj stronę</a>
        </div>
      </div>
      <img class="rounded-[8px] lg:max-w-[40rem] md:max-w-[30rem] xl:max-w-[50rem]" src="/clipboard.jpeg" alt="">
    </div>
  </div>
</template>
