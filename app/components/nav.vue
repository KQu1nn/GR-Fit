<template>
 <div class="fixed top-0 left-0 w-full flex justify-between items-center px-20 py-5 bg-neutral-900 text-white z-50 shadow-lg">
  <div class="flex flex-row gap-5 items-center cursor-pointer">
    <p class="font-sans italic text-2xl text-gray-200 font-bold">GR FIT <span class="text-red-500/90">Academia</span></p>
  </div>

  <ul class="flex flex-row gap-10 list-none text-md font-medium text-sm">
    <li class="cursor-pointer hover:text-red-500/90 hover:font-bold hover:scale-103 transition ease-in-out duration-100">Início</li>
    <li class="cursor-pointer hover:text-red-500/90 hover:font-bold hover:scale-103 transition ease-in-out duration-100">Matricule-se</li>
    <li class="cursor-pointer hover:text-red-500/90 hover:font-bold hover:scale-103 transition ease-in-out duration-100">Sobre nós</li>
    <li class="cursor-pointer hover:text-red-500/90 hover:font-bold hover:scale-103 transition ease-in-out duration-100">Contato</li>
  </ul>

  <button class="bg-red-500 text-sm font-bold px-5 py-2 cursor-pointer rounded-lg hover:scale-105 transition ease-in-out duration-300">
    Matricule-se agora
  </button>
</div>

</template>


<script setup>
import logo from '@/assets/images/logo.png'
</script>
