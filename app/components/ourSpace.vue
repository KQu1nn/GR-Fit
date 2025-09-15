<script setup lang="ts">
import { NuxtImg } from '#components';

</script>

<template>
  <div
    class="relative w-full min-h-[100dvh] bg-neutral-900 text-white flex flex-col gap-12 py-20 px-6 md:px-30 overflow-hidden">

    <div class="absolute inset-0 flex items-center justify-center">
      <div class="w-[400px] md:w-[500px] h-[400px] md:h-[500px] bg-red-500/40 blur-[50px] md:blur-[100px]"></div>
    </div>
    
    <div class="relative flex flex-col items-center gap-5 z-10 px-2">

      <h3 class="text-4xl md:text-5xl text-center font-bentham font-bold">Conheça <span class="text-red-500">nosso espaço</span></h3>
      <p class="w-11/12 md:w-4/6 text-center text-base md:text-lg text-gray-400">
        Na GR Fit, nosso espaço foi planejado para unir conforto, motivação e performance.
        Um ambiente moderno e acolhedor, pronto para impulsionar seus treinos e sua evolução.
      </p>
      <hr class="w-2/6 md:w-1/6 border-t-4 border-red-500 mt-3" />
    </div>

    <div
      class="w-full flex flex-col md:flex-row md:flex-wrap gap-6 relative z-10 pb-10 items-center md:items-stretch">
      <NuxtImg
        width="254"
        height="350"
        class="w-full md:w-auto h-auto md:h-[350px] object-cover rounded-md hover:scale-105 transition ease-in-out duration-300"
        src="/images/about.webp" alt="Nosso Espaçoo Academia" />
      <NuxtImg
        width="254"
        height="350"
        class="w-full md:w-auto h-auto md:h-[350px] object-cover rounded-md hover:scale-105 transition ease-in-out duration-300"
        src="/images/space1.webp" alt="Nosso Espaço Academia" />
      <NuxtImg
        width="254"
        height="350"
        class="w-full md:w-auto h-auto md:h-[350px] object-cover rounded-md hover:scale-105 transition ease-in-out duration-300"
        src="/images/space2.webp" alt="Nosso Espaço Academia" />
      <NuxtImg
        width="254"
        height="350"
        class="w-full md:w-auto h-auto md:h-[350px] object-cover rounded-md hover:scale-105 transition ease-in-out duration-300"
        src="/images/space3.webp" alt="Nosso Espaço Academia" />
    </div>
  </div>
</template>