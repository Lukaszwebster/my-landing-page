<script setup lang="ts">
const { t, locale } = useI18n()

// async function toggleLocales() {
//   // change to some real logic
//   const locales = availableLocales
//   const newLocale = locales[(locales.indexOf(locale.value) + 1) % locales.length]
//   await loadLanguageAsync(newLocale)
//   locale.value = newLocale
// }
</script>

<template>
  <div>
    <div class="ml-8 mr-8 mt-12 flex items-center justify-between">
      <div class="text-5">
        Moje<span class="font-1000">Logo</span>
      </div>
      <nav class="flex gap-2">
        <a href="https://github.com/Lukaszwebster">
          <img class="h-5 w-5" src="/github.svg" alt="">
        </a>

        <a href="https://www.linkedin.com/in/%C5%82ukasz-samcik-272222271/">
          <img class="h-5 w-5" src="/linkedin.svg" alt="">
        </a>

        <button :title="t('button.toggle_dark')" @click="toggleDark()">
          <div i="carbon-sun dark:carbon-moon" />
        </button>
      </nav>
    </div>
    <div class="ml-8 mr-8 mt-10">
      <h1 class="text-20px leading-tight">
        Siema. <br> <span class="text-30px font-extrabold"> Mam na imię Łukasz.</span> <br> Jestem początkującym frontend developerem.
      </h1>
      <h2 class="mt-10">
        Przez 8 lat pracowałem jako instruktor nauki jazdy kat. B oraz wykładowca nauki jazdy. Po tym czasie podjąłem decyzje o przebranżowieniu na stanowsko frontend developera. Naukę rozpocząłem 3 lata temu. Technologie z jakich korzystam i których się uczę to HTML, CSS, javascript, vue.js, tailwindcss, unocss, git.
      </h2>
    </div>
  </div>
</template>
