<script setup>
import { RouterLink } from 'vue-router'

const props = defineProps({
  title: {
    type: String,
  },
  subtitle: {
    type: String,
  },
  imgSrc: {
    type: String,
  },
  imgUrl: {
    type: String,
  },
  to: {
    type: String,
  },
  buttonText: {
    type: String,
  },
  class: {
    type: String,
  },
})
</script>

<template>
  <div class="mx-4 mt-20 items-center font-roboto 2xl:mx-[300px] lg:mx-[80px] md:mt-30">
    <div data-aos="fade-zoom-in" data-aos-offset="200" data-aos-easing="ease-in-sine" data-aos-duration="800" class="mt-20 flex flex-col items-center justify-center gap-3 md:mt-30">
      <h2 class="text-center text-[1.5rem] font-500">
        {{ props.title }}
      </h2>
      <h2 class="text-center leading-loose text-gray-500 md:max-w-800px md:text-left dark:text-gray-400">
        {{ props.subtitle }}
      </h2>
      <RouterLink class="button relative flex items-center gap-1 rounded-sm bg-gray-100 py-[0.2rem] pl-[1.2rem] pr-[1.4rem] transition-400 hover:bg-gray-200 dark:text-black" :to="props.to">
        {{ props.buttonText }}
        <div class="i-ic:baseline-arrow-right-alt arrow right-[1.4rem] transition-400" />
      </RouterLink>
      <picture class="mt-10 md:max-w-800px">
        <a :href="imgUrl">  <img :class="props.class" class="rounded-8px" :src="imgSrc" alt=""></a>
      </picture>
    </div>
  </div>
</template>

<style>
.button:hover > .arrow {
  transform: translate(0.5rem);
  }
</style>
