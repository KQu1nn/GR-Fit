<template>
  <div>
    <div
      class="w-full min-h-[100dvh] bg-gradient-to-tr from-neutral-900 via-neutral-900 to-red-900 text-white flex flex-col gap-12 md:gap-15 py-20 md:py-25 px-6 md:px-30">

      <div class="flex flex-col items-center gap-5 text-center">
        <span class="w-16 h-16 md:w-19 md:h-19 rounded-full bg-red-500 flex items-center justify-center">
          <Icon name="lucide:star" size="28" class="text-white md:size-32" />
        </span>
        <h3 class="text-3xl md:text-4xl font-bentham font-bold">Veja o que falam sobre nós</h3>

        <div class="flex flex-col items-center">
          <h3 class="text-2xl md:text-3xl font-black">4,7</h3>
          <div class="flex items-center my-1">

            <svg class="w-5 h-5 md:w-6 md:h-6 ms-2 text-yellow-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
              fill="currentColor" viewBox="0 0 22 20">
              <path
                d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
            </svg>
            <svg class="w-5 h-5 md:w-6 md:h-6 ms-2 text-yellow-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
              fill="currentColor" viewBox="0 0 22 20">
              <path
                d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
            </svg>
            <svg class="w-5 h-5 md:w-6 md:h-6 ms-2 text-yellow-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
              fill="currentColor" viewBox="0 0 22 20">
              <path
                d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
            </svg>
            <svg class="w-5 h-5 md:w-6 md:h-6 ms-2 text-yellow-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
              fill="currentColor" viewBox="0 0 22 20">
              <path
                d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
            </svg>
            <svg class="w-5 h-5 md:w-6 md:h-6 ms-2 text-gray-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
              fill="currentColor" viewBox="0 0 22 20">
              <path
                d="M20.924 7.625a1.523 1.523 0 0 0-1.238-1.044l-5.051-.734-2.259-4.577a1.534 1.534 0 0 0-2.752 0L7.365 5.847l-5.051.734A1.535 1.535 0 0 0 1.463 9.2l3.656 3.563-.863 5.031a1.532 1.532 0 0 0 2.226 1.616L11 17.033l4.518 2.375a1.534 1.534 0 0 0 2.226-1.617l-.863-5.03L20.537 9.2a1.523 1.523 0 0 0 .387-1.575Z" />
            </svg>
          </div>
          <p class="text-sm md:text-base">72 avaliações</p>
        </div>

        <hr class="w-2/6 md:w-1/6 border-t-4 border-red-500 mt-3" />
      </div>

      <div class="flex flex-col md:flex-row gap-6 md:gap-4 flex-wrap items-center md:items-stretch">
        <Article v-for="dataArticle in datasArticle" :dataArticle="dataArticle" :key="dataArticle.id" class="w-full md:w-[32%]" />

      </div>

    </div>
  </div>
</template>

<script setup>
import p1 from '@/assets/images/p1.webp'
import p2 from '@/assets/images/p2.webp'
import p3 from '@/assets/images/p3.webp'
const datasArticle = [
  {
    id: 1,
    name: 'Lusilaine Rios',
    avatar: p1,
    reviews: 103,
    time: '1 ano atrás',
    comment: 'Lugar agradável, organizado profissionais capacitados, nota 10.'
  },
  {
    id: 2,
    name: 'Itacuiris Oliveira (Íris)',
    avatar: p2,
    reviews: 22,
    time: '6 meses atrás',
    comment: `Foi muito bom! Um experiência que deixou gostinho de quero mais. super indico!!! 
Hoje sou cliente fiel...`
  },
  {
    id: 3,
    name: 'Suedna Priscila Rodrigues Moreira',
    avatar: p3,
    reviews: 76,
    time: '3 meses atrás',
    comment: 'Toda a equipe está de parabéns. Obrigada por esse atendimento diferenciado'
  }
]
</script>
