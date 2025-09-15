<template>
  <div class="w-full min-h-[100dvh] flex flex-col items-center bg-neutral-900 text-white py-14 md:py-25">
    <div class="flex flex-col items-center gap-5">
      <span class=" w-19 h-19 rounded-full bg-red-500 flex items-center justify-center">
        <Icon name="lucide:dumbbell" size="32" class="text-white" />
      </span>
      <h3 class="text-3xl md:text-4xl text-center font-bentham font-bold">Conheça nossos trabalhos</h3>
      <p class="w-10/12 md:w-4/6 text-center text-lg text-gray-400">Cada detalhe foi pensado para proporcionar a melhor experiência de treino. Venha conhecer nosso espaço onde sua transformação acontece.</p>
    </div>
    <div class="w-full min-h-[230px] flex flex-row flex-wrap justify-center gap-6 py-14 md:py-24 px-14">
      <WorksCard v-for="item in infosWorkCards" :key="item.id" :data="item" />
    </div>
    <div class="flex flex-col items-center gap-3">
        <button class="flex flex-row items-center justify-center gap-3 text-lg px-5 py-3 bg-green-500 rounded-md cursor-pointer hover:scale-105 transition ease-in-out duration-300">
          <Icon name="simple-icons:whatsapp" size="25" class="text-white" />
          <a href="https://api.whatsapp.com/send/?phone=5587991931948&text=Gostaria+de+saber+o+valor!">Converse no WhatsApp</a>
        </button>
        <p class="text-md text-gray-300 ">Tire suas dúvidas ou matricule-se</p>
      </div>
  </div>
</template>

<script setup>
import work1 from '@/assets/images/work1.webp'
import work2 from '@/assets/images/work2.webp'
import work3 from '@/assets/images/work3.webp'

const infosWorkCards = ref([
  { title: 'Musculação', description: 'Musculação fortalece os músculos, melhora a saúde cardiovascular e ajuda a prevenir doenças e quedas, mantendo seu corpo mais saudável e resistente.', image: work1, alt: 'musculação'},
  { title: 'Funcional ', description: 'O treino funcional melhora a força, flexibilidade e equilíbrio, ajudando na prevenção de lesões e promovendo um corpo mais ágil e saudável.', image: work2, alt: 'funcional'},
  { title: 'Fit Dance', description: 'Aulas de dança promovem bem-estar, melhoram coordenação e postura, fortalecem a autoestima e ajudam a reduzir o estresse.', image: work3, alt: 'fit-dance'}
])
</script>
