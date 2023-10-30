<script setup>
const { t, locale } = useI18n()
</script>

<template>
  <div class="mx-4 mt-12 flex items-center justify-between font-roboto 2xl:mx-[300px] lg:mx-[80px]">
    <a href="/" class="text-5">
      Łukasz<span class="font-1000">Samcik</span>
    </a>
    <nav class="flex gap-2 text-gray lg:gap-4">
      <a href="https://github.com/Lukaszwebster">
        <div class="i-mdi:github md:h-10 md:w-10 hover:text-black dark:hover:text-white" />
      </a>

      <a href="https://www.linkedin.com/in/%C5%82ukasz-samcik-272222271/">
        <div class="i-mdi:linkedin md:h-10 md:w-10 dark:text-gray hover:text-black dark:hover:text-white" />
      </a>
      <a href="https://codepen.io/Websterek">
        <div class="i-mdi:codepen md:h-10 md:w-10 hover:text-black dark:hover:text-white" />
      </a>

      <button :title="t('button.toggle_dark')" @click="toggleDark()">
        <div class="i-carbon-sun dark:i-carbon-moon hover:text-black md:!h-10 md:!w-10 dark:hover:text-white" />
      </button>
    </nav>
  </div>
</template>
