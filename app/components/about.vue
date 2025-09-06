<template>
  <div
    class="w-full min-h-[100dvh] bg-gradient-to-tr from-neutral-900 via-neutral-900 to-red-900 text-white flex flex-col gap-15 py-25 px-5 md:px-30">

    <div class="flex flex-col items-center gap-5">
      <span class="w-19 h-19 rounded-full bg-red-500 flex items-center justify-center">
        <Icon name="lucide:biceps-flexed" size="32" class="text-white" />
      </span>
      <h3 class="text-3xl md:text-4xl text-center font-bentham font-bold">Sobre nós</h3>
      <p class="w-11/12 md:w-4/6 text-center text-base md:text-lg text-gray-400">
        Na GR Fit, nosso espaço foi planejado para unir conforto, motivação e performance.
        Um ambiente moderno e acolhedor, pronto para impulsionar seus treinos e sua evolução.
      </p>
      <hr class="w-1/6 border-t-2 border-red-500 mt-3" />
    </div>

    <div class="md:py-20 md:px-10 flex flex-col md:flex-row gap-10 md:gap-20 items-center md:items-start">
      <img :src="aboutImage" alt="GR FIT" class="w-full max-w-[420px] h-auto rounded-lg md:h-[520px] object-cover" />

      <div class="flex flex-col justify-center gap-6 text-gray-300 text-base md:text-md text-center md:text-left">
        <h1 class="text-3xl md:text-4xl text-white">Quem é a GRFIT?</h1>
        <p class="w-full leading-relaxed">
          A GRFIT Academia, localizada em Petrolina, foi criada para todos os públicos.
          Aqui você encontra musculação profissional, avaliação personalizada e aulas de dança que inspiram.
          <br><br>
          Mais do que uma academia, somos um espaço de acolhimento, força e evolução, com profissionais
          qualificados para acompanhar cada etapa da sua jornada.
          <br><br>
          Na GRFIT, cada treino tem um propósito e cada pessoa é única. Nossa energia vive em quem chega e
          floresce em quem decide ficar.
          <br><br>
          <span class="font-bold text-white">GRFIT Academia</span><br />
          Seu corpo, sua mente, sua melhor versão. Todos os dias.
          <br><br>
          Oferecemos uma experiência de alto valor, com preços justos e uma estrutura excepcional.
          <br>
          Venha fazer parte da GR Fit e transforme sua jornada de treino conosco!
        </p>

        <div class="w-full flex flex-col gap-3">
          <p class="text-lg font-bold">Localização e Contato</p>
          <div class="flex flex-wrap justify-center md:justify-start gap-4 mt-2">
            <a
              href="https://www.google.com/maps/place/GR+FIT+ACADEMIA/@-9.3558788,-40.5001942,15z/data=!4m15!1m8!3m7!1s0x7737aeef7e980bb:0xa3da4d4bd46371!2sR.+do+M%C3%A1rmore+-+Petrolina,+PE!3b1!8m2!3d-9.3547177!4d-40.500205!16s%2Fg%2F1ymxdxh6q!3m5!1s0x7737b93f4b6ce6f:0x44b5d5535f253c75!8m2!3d-9.3540765!4d-40.4911714!16s%2Fg%2F11qzfz5l_s?entry=ttu&g_ep=EgoyMDI1MDkwMy4wIKXMDSoASAFQAw%3D%3D">
              <Icon name="lucide:map-pin" size="28"
                class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 text-red-500/80" />
            </a>
            <a href="https://api.whatsapp.com/send/?phone=5587991931948&text=Gostaria+de+saber+o+valor!">
              <Icon name="lucide:phone" size="28"
                class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 text-red-500/80" />
            </a>
            <a href="https://www.instagram.com/grfit.academia">
              <Icon name="lucide:instagram" size="28"
                class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 text-red-500/80" />
            </a>

            <Icon name="lucide:mail" size="28"
              class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 text-red-500/80" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import aboutImage from '@/assets/images/about.jpeg'
</script>
