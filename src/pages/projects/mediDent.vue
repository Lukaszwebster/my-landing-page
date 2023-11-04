<script setup>
const techItems = ['vue', 'UnoCss']
</script>

<template>
  <div class="mx-4 mt-12 font-roboto 2xl:mx-[300px] lg:mx-[80px]">
    <div class="">
      <div class="max-w-[40rem]">
        <h1 class="text-[1.8rem] font-500">
          MediDent
        </h1>
        <h2 class="text-gray">
          Gabinet stomatologiczny
        </h2>
        <p class="mt-12 text-gray">
          MediDent to zaprzyjaźniony gabinet stomatologiczny. Gdy tylko dowiedziałem się, że firmie potrzebna jest strona internetowa postanowiłem nie odpłatnie ją wykonać. Praca nad projektem była ciekawym doświadczeniem.
        </p>
      </div>
      <div class="mt-[4rem] w-full flex flex-col justify-between gap-4 md:flex-row">
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
            <a class="underline" href="https://medidentpulawy.pl/">Obejrzyj stronę</a>
          </div>
        </div>
        <img class="rounded-[8px] lg:max-w-[40rem] md:max-w-[30rem] xl:max-w-[50rem]" src="/MediDentImg.png" alt="">
      </div>
      <div class="mt-[2rem] max-w-[40rem] flex flex-col gap-4">
        <h2 class="text-[1.5rem] font-500">
          Szczegóły
        </h2>
        <p class="text-gray">
          Przy pracy ze strona MediDent napotkałem wiele wyzwań ponieważ projekt musiał być stworzony od początku do końca. oznaczało to, że do mnie należało wybranie technologii, wymyślenie wyglądu strony, wykonanie zdjęć w firmie oraz teksty. Uświadomiło mi to jak trudne jest wykonanie wszystkiego samodzielnie i jak bardzo w innych projektach liczą się role poszczególnych członków teamu.
        </p>
      </div>
    </div>
  </div>
</template>
