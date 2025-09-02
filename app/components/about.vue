<template>
    <div
        class="w-full min-h-[100dvh] bg-gradient-to-tr from-neutral-900 via-neutral-900 to-red-900 text-white flex flex-col gap-15 py-25 px-30">

        <div class="flex flex-col items-center gap-5">
            <span class=" w-19 h-19 rounded-full bg-red-500 flex items-center justify-center">
                <Icon name="lucide:biceps-flexed" size="32" class="text-white" />
            </span>
            <h3 class="text-4xl text-center font-bentham font-bold">Sobre nós</h3>
            <p class="w-4/6 text-center text-lg text-gray-400">Na GR Fit, nosso espaço foi planejado para unir conforto,
                motivação e performance. Um ambiente moderno e acolhedor, pronto para impulsionar seus treinos e sua
                evolução.</p>
            <hr class="w-1/6 border-t-2 border-red-500 mt-3" />
        </div>

        <div class="py-20 px-10 flex flex-row gap-20 ">
            <img :src="aboutImage" alt="GR FIT" class="h-[520px]">
            <div class=" flex flex-col justify-center gap-6 text-md text-gray-300">
                <h1 class="text-4xl text-white">Quem é a GRFIT?</h1>
                <p class="w-full ">
                    A GRFIT Academia, localizada em Petrolina, foi criada para todos os públicos.
                    Aqui você encontra musculação profissional, avaliação personalizada e aulas de dança que inspiram.
                    <br><br>
                    Mais do que uma academia, somos um espaço de acolhimento, força e evolução, com profissionais
                    qualificados para acompanhar cada etapa da sua jornada.
                    <br><br>
                    Na GRFIT, cada treino tem um propósito e cada pessoa é única. Nossa energia vive em quem chega e
                    floresce em quem decide ficar.
                    <br><br>
                    GRFIT Academia
                    Seu corpo, sua mente, sua melhor versão. Todos os dias.
                    <br><br>
                    Oferecemos uma experiência de alto valor, com preços justos e uma estrutura excepcional.
                    <br>
                    Venha fazer parte da GR Fit e transforme sua jornada de treino conosco!
                </p>
                <div class="w-full flex flex-col gap-3">
                    <p class="text-lg font-bold">Localização e Contato</p>
                    <div class="flex flex-row gap-4">
                        <Icon name="lucide:map-pin" size="30" class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 inline text-red-500/80 mr-2" />
                        <Icon name="lucide:phone" size="30" class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 inline text-red-500/80 mr-2" />
                        <Icon name="lucide:instagram" size="30" class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 inline text-red-500/80 mr-2" />
                        <Icon name="lucide:mail" size="30" class="cursor-pointer hover:scale-110 transition ease-in-out duration-200 inline text-red-500/80 mr-2" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
import aboutImage from '@/assets/images/about.jpeg'
</script>