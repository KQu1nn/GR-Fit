<template>
<div class="relative w-full min-h-[100dvh] bg-neutral-900 flex flex-col overflow-hidden pt-[80px]">
  <span aria-hidden="true" class="pointer-events-none absolute top-1/2 -translate-y-1/2 -right-70 h-[32rem] w-[32rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />
  <span aria-hidden="true" class="pointer-events-none absolute -top-30 -left-55 h-[35rem] w-[28rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />
  <Nav />
  <div class="relative z-20 flex flex-row items-start px-35 w-full flex-1">
    <div class="w-3/6 my-auto flex flex-col gap-8 items-start">
      <h1 class="w-11/12 font-bentham font-bold text-7xl text-white">
        Transforme seu corpo. Eleve sua mente.
      </h1>
      <p class="w-8/12 text-gray-300 text-xl">
        Na GR FIT, ajudamos você a encontrar seu equilíbrio entre força e mente.
      </p>
      <button class="bg-red-500 text-lg font-bold px-10 py-4 rounded-xl hover:scale-105 transition ease-in-out duration-300">
        Matricule-se agora
      </button>
    </div>
    <img :src="heroImage" class="absolute bottom-0 right-30 h-[700px] w-auto object-contain" />
  </div>
</div>


</template>

<script setup>
import heroImage from '@/assets/images/hero-image.png'
</script>
