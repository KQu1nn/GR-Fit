<template>
    <div class="w-full min-h-[100dvh] bg-gradient-to-tr from-neutral-900 via-neutral-900 to-red-900 text-white flex flex-col gap-15 py-25 px-30">
        
        <div class="flex flex-col items-center gap-5">
            <span class=" w-20 h-20 rounded-full bg-red-500 flex items-center justify-center">
                <Icon name="lucide:biceps-flexed" size="38" class="text-white" />
            </span>
            <h3 class="text-5xl text-center font-bentham font-bold">Sobre nós</h3>
            <p class="w-4/6 text-center text-xl text-gray-400">Na GR Fit, nosso espaço foi planejado para unir conforto,
                motivação e performance. Um ambiente moderno e acolhedor, pronto para impulsionar seus treinos e sua
                evolução.</p>
            <hr class="w-1/6 border-t-2 border-red-500 mt-3" />
        </div>

        <div class="py-15 px-30 flex flex-row gap-20 ">
            <img :src="aboutImage" alt="GR FIT" class="h-[600px]">
            <div class=" flex flex-col justify-center gap-15 text-lg text-gray-300">
                <h1 class="text-5xl text-white">Quem é a GRFIT?</h1>
                <p class="w-11/12">
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
            </div>
        </div>
    </div>
</template>
<script setup>
import aboutImage from '@/assets/images/about.jpeg'
</script>