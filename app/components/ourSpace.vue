<template>
  <div class="relative w-full min-h-[100dvh] bg-neutral-900  text-white flex flex-col gap-15 py-20 px-30 overflow-hidden">

    <div class="absolute inset-0 flex items-center justify-center">
      <div class="w-[500px] h-[500px] bg-red-500/40 blur-[100px] rounded-full"></div>
    </div>

    <div class="relative flex flex-col items-center gap-5 z-10">
      <h3 class="text-5xl text-center font-bentham font-bold">Conheça nosso espaço</h3>
      <p class="w-4/6 text-center text-lg text-gray-400">
        Na GR Fit, nosso espaço foi planejado para unir conforto, motivação e performance. 
        Um ambiente moderno e acolhedor, pronto para impulsionar seus treinos e sua evolução.
      </p>
      <hr class="w-1/6 border-t-4 border-red-500 mt-3" />
    </div>
    <div class="w-full flex flex-row flex-wrap gap-4 relative z-10 pb-15">
      <img class="h-[350px] hover:scale-105 transition ease-in-out duration-300" :src="spaceImage1">
      <img class="h-[350px] hover:scale-105 transition ease-in-out duration-300" :src="spaceImage2">
      <img class="h-[350px] hover:scale-105 transition ease-in-out duration-300" :src="aboutImage">
      <img class="h-[350px] hover:scale-105 transition ease-in-out duration-300" :src="spaceImage3">
    </div>
  </div>
</template>
<script setup>
import aboutImage from '@/assets/images/about.jpeg'
import spaceImage1 from '@/assets/images/space1.jpeg'
import spaceImage2 from '@/assets/images/space2.jpeg'
import spaceImage3 from '@/assets/images/space3.jpg'
</script>