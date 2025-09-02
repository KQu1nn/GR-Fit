<template>
  <div class="w-full min-h-[100dvh] flex flex-col items-center bg-neutral-900 text-white py-25">
    <div class="flex flex-col items-center gap-5">
      <span class=" w-20 h-20 rounded-full bg-red-500 flex items-center justify-center">
        <Icon name="lucide:dumbbell" size="38" class="text-white" />
      </span>
      <h3 class="text-5xl text-center font-bentham font-bold">Conheça nossos trabalhos</h3>
      <p class="w-4/6 text-center text-xl text-gray-400">Cada detalhe foi pensado para proporcionar a melhor experiência de treino. Venha conhecer nosso espaço onde sua transformação acontece.</p>
    </div>
    <div class="w-full flex flex-row justify-between gap-6 py-25 px-30">
      <WorksCard :infosWorkCards="infosWorkCards" />
    </div>
    <div class="flex flex-col items-center gap-3">
        <button class="flex flex-row items-center justify-center gap-3 text-lg px-5 py-3 bg-green-500 rounded-md cursor-pointer hover:scale-105 transition ease-in-out duration-300">
          <Icon name="simple-icons:whatsapp" size="28" class="text-white" />
          Converse no WhatsApp
        </button>
        <p class="text-lg text-gray-300 ">Tire suas dúvidas ou matricule-se</p>
      </div>
  </div>
</template>

<script setup>
import work1 from '@/assets/images/work1.jpg'
import work2 from '@/assets/images/work2.avif'
import work3 from '@/assets/images/work3.png'

const infosWorkCards = ref([
  { title: 'Musculação', description: 'Musculação fortalece os músculos, melhora a saúde cardiovascular e ajuda a prevenir doenças e quedas, mantendo seu corpo mais saudável e resistente.', image: work1},
  { title: 'Funcional ', description: 'O treino funcional melhora a força, flexibilidade e equilíbrio, ajudando na prevenção de lesões e promovendo um corpo mais ágil e saudável.', image: work2},
  { title: 'Fit Dance', description: 'Aulas de dança promovem bem-estar, melhoram coordenação e postura, fortalecem a autoestima e ajudam a reduzir o estresse.', image: work3}
])
</script>
