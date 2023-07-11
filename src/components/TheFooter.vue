<script setup>
import { availableLocales, loadLanguageAsync } from '~/modules/i18n'

const { t, locale } = useI18n()

async function toggleLocales() {
  // change to some real logic
  const locales = availableLocales
  const newLocale = locales[(locales.indexOf(locale.value) + 1) % locales.length]
  await loadLanguageAsync(newLocale)
  locale.value = newLocale
}
</script>

<template>
  <!-- <nav flex="~ gap-4" mt-6 justify-center text-xl>
    <RouterLink icon-btn to="/" :title="t('button.home')">
      <div i-carbon-campsite />
    </RouterLink>

    <button icon-btn :title="t('button.toggle_dark')" @click="toggleDark()">
      <div i="carbon-sun dark:carbon-moon" />
    </button>

    <a icon-btn :title="t('button.toggle_langs')" @click="toggleLocales()">
      <div i-carbon-language />
    </a>

    <RouterLink icon-btn to="/about" :title="t('button.about')">
      <div i-carbon-dicom-overlay />
    </RouterLink>

    <a icon-btn rel="noreferrer" href="https://github.com/antfu/vitesse" target="_blank" title="GitHub">
      <div i-carbon-logo-github />
    </a>
  </nav> -->
  <div class="mt-10 h-[200px] bg-myBlue pt-10">
    <div class="flex items-center justify-center gap-4">
      <div>
        l.samcik@gmail.com
      </div>
      <nav class="flex gap-2 text-gray">
        <a href="https://github.com/Lukaszwebster">
          <div class="i-mdi:github md:h-10 md:w-10 hover:text-black dark:hover:text-white" />
        </a>

        <a href="https://www.linkedin.com/in/%C5%82ukasz-samcik-272222271/">
          <div class="i-mdi:linkedin md:h-10 md:w-10 dark:text-gray hover:text-black dark:hover:text-white" />
        </a>
        <a href="https://codepen.io/Websterek">
          <div class="i-mdi:codepen md:h-10 md:w-10 hover:text-black dark:hover:text-white" />
        </a>
      </nav>
    </div>
  </div>
</template>
