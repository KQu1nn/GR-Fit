<template>
  <div id="contato"
    class="relative w-full min-h-[100dvh] bg-neutral-900 text-white flex flex-col gap-15 py-15 px-5 md:px-20 overflow-hidden">
    <div class="absolute inset-0 flex items-center justify-center z-0">
      <div class="w-[500px] h-[500px] bg-red-500/30 blur-[100px] rounded-full"></div>
    </div>

    <div class="flex flex-col items-center gap-5 relative z-10 px-3 text-center">
      <span class="w-16 h-16 md:w-19 md:h-19 rounded-full bg-red-500 flex items-center justify-center">
        <Icon name="lucide:phone" size="28" class="text-white md:size-32" />
      </span>
      <h3 class="text-3xl md:text-4xl font-bold">
        Vamos <span class="text-red-500">conversar?</span>
      </h3>
      <p class="w-full md:w-4/6 text-lg text-gray-400">
        Estamos aqui para ajudar você a dar o primeiro passo na sua jornada de transformação. Entre em contato conosco!
      </p>
      <hr class="w-2/6 md:w-1/6 border-t-4 border-red-500 mt-3" />
    </div>

    <div class="flex flex-col md:flex-row justify-center items-center gap-8 md:gap-12 relative z-10">
      <div class="flex flex-col md:flex-row md:flex-wrap gap-5 w-full md:w-auto justify-center items-center">
  <ContactCard v-for="dataContact in dataContacts" :key="dataContact.title" :dataContact="dataContact" />
</div>


      <div
        class="w-full h-[300px] md:w-[700px] md:h-[450px] bg-transparent rounded-lg flex flex-col items-center justify-center text-red-500 font-bold">
        <h2 class="pb-4 text-lg md:text-xl flex items-center">
          <Icon name="lucide:map-pin" size="18" class="inline-block mr-2 md:size-20" />
          Localização
        </h2>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3982.409804060616!2d-40.51863588405094!3d-9.392285990579908!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x785737b6f3a2c9ff%3A0x2a7caa4a3c1f1a99!2sR.%20da%20Caridade%2C%20Dom%20Avelar%2C%20Petrolina%20-%20PE%2C%2056323-540!5e0!3m2!1spt-BR!2sbr!4v1693675000000!5m2!1spt-BR!2sbr"
          width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"
          referrerpolicy="no-referrer-when-downgrade">
        </iframe>
      </div>
    </div>
  </div>

  <div class="flex flex-col items-center gap-5 pt-10 bg-neutral-800 text-white py-10 relative z-10">
    <h2 class="text-2xl md:text-3xl font-bold">Pronto para <span class="text-red-500">começar?</span></h2>
    <p class="text-md md:text-lg text-center w-5/6 md:w-3/6 text-gray-300">
      <span class="font-bold">Agende</span> sua visita e conheça pessoalmente tudo o que a <span class="font-bold">GRFIT</span> pode oferecer para sua <span class="font-bold">transformação.</span>
    </p>
    <div class="flex flex-col items-center gap-3">
      <button
        class="flex flex-row items-center justify-center gap-3 text-md md:text-lg px-5 py-3 bg-green-500 rounded-md cursor-pointer hover:scale-105 transition ease-in-out duration-300">
        <Icon name="simple-icons:whatsapp" size="24" class="text-white md:size-28" />
        <a href="https://wa.me/5599999999999">Converse no WhatsApp</a>
      </button>
      <p class="text-sm md:text-md text-gray-300">Tire suas dúvidas ou matricule-se</p>
    </div>
  </div>
</template>

<script setup>
const dataContacts = ref([
  {
    icon: 'lucide:map-pin',
    title: 'Localização',
    description: 'R. da Caridade',
    subdescription: 'Dom Avelar, Petrolina - PE',
    button: 'Ver no maps',
    url: 'https://www.google.com/maps/place/GR+FIT+ACADEMIA/@-9.3558788,-40.5001942,15z/data=!4m15!1m8!3m7!1s0x7737aeef7e980bb:0xa3da4d4bd46371!2sR.+do+M%C3%A1rmore+-+Petrolina,+PE!3b1!8m2!3d-9.3547177!4d-40.500205!16s%2Fg%2F1ymxdxh6q!3m5!1s0x7737b93f4b6ce6f:0x44b5d5535f253c75!8m2!3d-9.3540765!4d-40.4911714!16s%2Fg%2F11qzfz5l_s?entry=ttu&g_ep=EgoyMDI1MDkwMy4wIKXMDSoASAFQAw%3D%3D',
  },
  {
    icon: 'lucide:phone',
    title: 'Telefone',
    description: '(87) 99195-0269',
    subdescription: 'WhatsApp disponível',
    button: 'Ligar agora',
    url: 'https://wa.me/5599999999999',
  },
  {
    icon: 'lucide:clock',
    title: 'Horários',
    description: 'Seg-Sex: 6h às 23h',
    subdescription: 'Sáb: 7h às 20h | Dom: 8h às 18h',
    button: 'Ver Horarios',
    url: '',
  },
  {
    icon: 'lucide:instagram',
    title: 'Instagram',
    description: '@grfit.academia',
    subdescription: 'Siga-nos para novidades',
    button: 'Seguir no instagram',
    url: 'https://www.instagram.com/grfit.academia',
  }
])
</script>
