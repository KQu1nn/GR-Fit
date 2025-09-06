<template>
  <div data-header
    class="fixed top-0 left-0 w-full flex justify-between items-center px-5 md:px-20 py-5 bg-neutral-900 text-white z-50 shadow-lg">
    <div class="flex flex-row gap-5 items-center cursor-pointer">
      <p class="font-sans italic text-2xl text-gray-200 font-bold cursor-pointer" @click="goToSection('inicio')">
        GR FIT <span class="text-red-500/90">Academia</span>
      </p>
    </div>

    <ul class="hidden md:flex flex-row gap-10 list-none text-md font-medium text-sm">
      <li v-for="item in menu" :key="item.id" @click="goToSection(item.id)"
        class="cursor-pointer hover:text-red-500/90 hover:font-bold hover:scale-103 transition ease-in-out duration-100">
        {{ item.label }}
      </li>
    </ul>

    <button
      class="hidden md:block bg-red-500 text-sm font-bold px-5 py-2 cursor-pointer rounded-lg hover:scale-105 transition ease-in-out duration-300">
      <a href="https://api.whatsapp.com/send/?phone=5587991931948&text=Gostaria+de+saber+o+valor!">Matricule-se agora</a>
    </button>

    <button class="md:hidden flex flex-col gap-1 cursor-pointer" @click="toggleMenu">
      <span class="w-6 h-0.5 bg-white transition" :class="{ 'rotate-45 translate-y-1.5': isOpen }" />
      <span class="w-6 h-0.5 bg-white transition" :class="{ 'opacity-0': isOpen }" />
      <span class="w-6 h-0.5 bg-white transition" :class="{ '-rotate-45 -translate-y-1.5': isOpen }" />
    </button>

    <transition name="slide-fade">
      <div v-if="isOpen"
        class="absolute top-full left-0 w-full bg-neutral-900 shadow-lg flex flex-col items-center gap-5 py-6 md:hidden">
        <ul class="flex flex-col gap-6 text-lg font-medium list-none">
          <li v-for="item in menu" :key="item.id" @click="() => { goToSection(item.id); toggleMenu() }"
            class="cursor-pointer hover:text-red-500/90 hover:font-bold transition ease-in-out duration-100">
            {{ item.label }}
          </li>
        </ul>
        <button
          class="bg-red-500 text-sm font-bold px-5 py-2 cursor-pointer rounded-lg hover:scale-105 transition ease-in-out duration-300">
          <a href="https://api.whatsapp.com/send/?phone=5587991931948&text=Gostaria+de+saber+o+valor!">Matricule-se agora</a>
        </button>
      </div>
    </transition>
  </div>
</template>

<script setup>
import { ref } from "vue"

const isOpen = ref(false)

function toggleMenu() {
  isOpen.value = !isOpen.value
}

const menu = [
  { id: "inicio", label: "Início" },
  { id: "trabalhos", label: "Trabalhos" },
  { id: "sobre", label: "Sobre nós" },
  { id: "espaco", label: "Espaço" },
  { id: "avaliacoes", label: "Avaliações" },
  { id: "contato", label: "Contato" },
]

function goToSection(id) {
  const el = document.getElementById(id)
  if (!el) {
    console.warn(`Seção com id="${id}" não encontrada.`)
    return
  }

  const header = document.querySelector("[data-header]")
  const headerHeight = header ? header.offsetHeight : 0

  const top = el.getBoundingClientRect().top + window.scrollY - headerHeight
  window.scrollTo({ top, behavior: "smooth" })
}
</script>

<style scoped>
.slide-fade-enter-active,
.slide-fade-leave-active {
  transition: all 0.3s ease;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  opacity: 0;
  transform: translateY(-10px);
}
</style>
