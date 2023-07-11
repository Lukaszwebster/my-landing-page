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
  <div class="mx-4">
    <div class="mt-12 flex items-center justify-between">
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
    <div class="mt-10">
      <div class="sm:flex sm:justify-between">
        <picture class="max-w-500px">
          <img class="rounded-4px" src="/zdjecie-ja-2.jpeg" alt="">
        </picture>
        <div class="sm:ml-4 sm:max-w-400px">
          <h1 class="mt-10 text-28px leading-tight sm:mt-0 sm:text-right">
            Siema. <br> <span class="text-28px font-extrabold"> Mam na imię Łukasz.</span> <br> <span class="text-30px">Jestem początkującym frontend developerem.</span>
          </h1>

          <h2 class="mt-10 leading-loose text-gray sm:text-right">
            Przez 8 lat pracowałem jako instruktor nauki jazdy kat. B oraz wykładowca nauki jazdy. <br> Po tym czasie podjąłem decyzje o przebranżowieniu na stanowsko frontend developera. Naukę rozpocząłem 3 lata temu. Z poszerzania wiedzy oraz pracy nad projektami czerpię duzo przyjemnosci i satysfakcji. Technologie z jakich korzystam i których się uczę to HTML, CSS, Javacript, vue.js, tailwindcss, unocss, git.
          </h2>
        </div>
      </div>
    </div>
  </div>
</template>
