<script setup>
const props = defineProps({
  title: {
    type: String,
  },
  subtitle: {
    type: String,
  },
  description: {
    type: String,
  },
  imgUrl: {
    type: String,
  },
  href: {
    type: String,
  },
  skills: {
    type: Array,
  },
  details: {
    type: String,
  },
  imgStyle: {
    type: String,
  },
})
</script>

<template>
  <div class="mx-4 mt-12 font-roboto 2xl:mx-[300px] lg:mx-[80px]">
    <div class="max-w-[40rem]">
      <h1 class="text-[1.8rem] font-500">
        {{ props.title }}
      </h1>
      <h2 class="text-gray-500 dark:text-gray-400">
        {{ props.subtitle }}
      </h2>
      <p class="mt-12 text-gray-500 dark:text-gray-400">
        {{ props.description }}
      </p>
    </div>
    <div class="mt-[4rem] w-full flex flex-col justify-between gap-4 md:flex-row">
      <div>
        <h2 class="text-gray-500 dark:text-gray-400">
          Technologie w projekcie
        </h2>
        <div class="mt-[2rem] flex flex-col gap-1">
          <ul v-for="(item, index) in skills" :key="index">
            <li class="inline-block cursor-default rounded-4px bg-#fafafa px-2 py-1 hover:bg-gray dark:text-black">
              {{ item }}
            </li>
          </ul>
        </div>
        <div class="mt-[2rem]">
          <a class="underline" :href="props.href">Obejrzyj stronę</a>
        </div>
      </div>
      <img :class="imgStyle" class="rounded-[8px] lg:max-w-[40rem] md:max-w-[30rem] xl:max-w-[50rem]" :src="props.imgUrl" alt="">
    </div>
    <div class="mt-[2rem] max-w-[40rem] flex flex-col gap-4">
      <h2 class="text-[1.5rem] font-500">
        Szczegóły
      </h2>
      <p class="text-gray-500 dark:text-gray-400">
        {{ props.details }}
      </p>
    </div>
  </div>
</template>
