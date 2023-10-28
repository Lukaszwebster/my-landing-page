<script setup>
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
})
</script>

<template>
  <div class="mx-4 mt-20 items-center font-roboto 2xl:mx-[300px] lg:mx-[80px] md:mt-30">
    <div data-aos="fade-zoom-in" data-aos-offset="200" data-aos-easing="ease-in-sine" data-aos-duration="800" class="mt-20 flex flex-col items-center justify-center md:mt-30">
      <h2 class="text-center text-[1.5rem]">
        {{ props.title }}
      </h2>
      <h2 class="class= mt-4 text-center leading-loose text-gray md:max-w-800px md:text-left">
        {{ props.subtitle }}
      </h2>
      <button class="bg-gray-200">
        O projekcie
      </button>
      <picture class="mt-10 md:max-w-800px">
        <a :href="imgUrl">  <img class="rounded-8px" :src="imgSrc" alt=""></a>
      </picture>
    </div>
  </div>
</template>
