<template>
  <div class="relative w-full min-h-[100dvh] bg-neutral-900 flex flex-col overflow-hidden pt-[80px]">
    <span
      aria-hidden="true"
      class="pointer-events-none absolute top-1/2 -translate-y-1/2 -right-70 h-[32rem] w-[32rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />
    <span
      aria-hidden="true"
      class="pointer-events-none absolute -top-30 -left-55 h-[35rem] w-[28rem] rounded-full blur-[100px] opacity-100 bg-[radial-gradient(closest-side,theme(colors.red.500),transparent_90%)] z-0" />

    <Nav />

    <div class="relative z-20 flex flex-col md:flex-row items-center md:items-start px-6 md:px-35 w-full flex-1 gap-10 md:gap-0">
      
      <div class="w-full md:w-3/6 my-auto flex flex-col gap-6 md:gap-5 items-center md:items-start text-center md:text-left relative z-20">
        <h1 class="w-full md:w-11/12 font-bentham font-bold text-5xl md:text-6xl text-white leading-snug md:leading-14">
          Mais que uma academia, uma jornada.
        </h1>
        <p class="w-10/12 md:w-8/12 text-gray-300 text-base md:text-lg">
          Na GR FIT, você supera limites e descobre o seu verdadeiro potencial.
        </p>
        <div class="flex flex-col md:flex-row gap-5 md:gap-8 items-center">
          <button aria-labels="matricule-se"
            class="bg-red-500 text-md text-white font-bold cursor-pointer px-6 py-3 rounded-lg hover:scale-105 transition ease-in-out duration-300 w-full md:w-auto">
            <a href="https://api.whatsapp.com/send/?phone=5587991931948&text=Gostaria+de+saber+o+valor!">Matricule-se agora</a>
          </button>
          <button aria-labels="mapa"
            class="bg-neutral-900 shadow-md border-2 border-red-500 text-md text-red-500 flex items-center justify-center cursor-pointer font-bold px-6 py-3 rounded-xl hover:scale-105 transition ease-in-out duration-300 w-full md:w-auto">
            <Icon name="lucide:map-pin" size="24" class="inline text-red-500 mr-2" />
            <a href="https://www.google.com/maps/place/GR+FIT+ACADEMIA/@-9.3558788,-40.5001942,15z/data=!4m15!1m8!3m7!1s0x7737aeef7e980bb:0xa3da4d4bd46371!2sR.+do+M%C3%A1rmore+-+Petrolina,+PE!3b1!8m2!3d-9.3547177!4d-40.500205!16s%2Fg%2F1ymxdxh6q!3m5!1s0x7737b93f4b6ce6f:0x44b5d5535f253c75!8m2!3d-9.3540765!4d-40.4911714!16s%2Fg%2F11qzfz5l_s?entry=ttu&g_ep=EgoyMDI1MDkwMy4wIKXMDSoASAFQAw%3D%3D">Localização</a>
          </button>
        </div>
      </div>

      <img
        :src="heroImage"
        class="absolute md:relative inset-0 md:inset-auto mx-auto md:mx-0 h-[320px] md:h-[570px] w-auto object-contain opacity-20 md:opacity-100 z-10 md:z-5" />
    </div>

    <div class="absolute bottom-6 left-1/2 -translate-x-1/2 z-30">
      <Icon name="lucide:chevron-down" size="40" class="text-white animate-bounce" />
    </div>
  </div>
</template>

<script setup>
import heroImage from '@/assets/images/hero-image.webp'
</script>
