<script setup>
const techItems = ['vue', 'unoCss']
</script>

<template>
  <div class="mx-4 mt-12 font-roboto 2xl:mx-[300px] lg:mx-[80px]">
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
      <div class="mt-[4rem]">
        <h2>Technologie z których korzystałem</h2>
        <div class="mt-[2rem]">
          <ul v-for="(item, index) in techItems" :key="index">
            <li class="w-min rounded-4px bg-#fafafa px-2 py-1 hover:bg-gray">
              {{ item }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
