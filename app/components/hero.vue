<template>
  <div class="relative w-full min-h-[100dvh] bg-neutral-900 flex flex-col overflow-hidden pt-[80px]">
    <span aria-hidden="true"
      class="pointer-events-none absolute top-1/2 -translate-y-1/2 -right-70 h-[32rem] w-[32rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />
    <span aria-hidden="true"
      class="pointer-events-none absolute -top-30 -left-55 h-[35rem] w-[28rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />
    <Nav />
    <div class="relative z-20 flex flex-row items-start px-35 w-full flex-1">
      <div class="w-3/6 my-auto flex flex-col gap-8 items-start">
        <h1 class="w-11/12 font-bentham font-bold text-6xl text-white">
          Transforme seu corpo. Eleve sua mente.
        </h1>
        <p class="w-8/12 text-gray-300 text-lg">
          Na GR FIT, ajudamos você a encontrar seu equilíbrio entre força e mente.
        </p>
        <div class="flex flex-row gap-8 items-center">
          <button
            class="bg-red-500 text-md text-white font-bold cursor-pointer px-5 py-3 rounded-lg hover:scale-105 transition ease-in-out duration-300">
            Matricule-se agora
          </button>
          <button class="bg-neutral-900 shadow-md border-2 border-red-500 text-md text-red-500 flex items-center cursor-pointer font-bold px-5 py-2 rounded-xl hover:scale-105 transition ease-in-out duration-300">
            <Icon name="lucide:map-pin" size="28" class="inline text-red-500 mr-2" />
            Localização
          </button>
        </div>
      </div>
      <img :src="heroImage" class="absolute bottom-0 right-30 h-[570px] w-auto object-contain" />
    </div>
  </div>


</template>

<script setup>
import heroImage from '@/assets/images/hero-image.png'
</script>
