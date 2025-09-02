<template>
  <footer class="w-full px-5 py-10 md:px-20 bg-neutral-900 text-white flex flex-col gap-10">

    <div class="flex flex-col md:flex-row md:justify-between gap-10 md:gap-20">
      
      <div class="flex flex-col gap-5 items-center md:items-start text-center md:text-left md:w-1/3">
        <p class="font-sans italic text-xl font-bold">
          GR FIT <span class="text-red-500">Academia</span>
        </p>
        <p class="text-gray-300 text-sm">
          Mais que uma academia. Somos um espaço de acolhimento, força e evolução. Na GRFIT, cada treino tem um propósito. E cada pessoa é única.
        </p>
        <div class="flex flex-row justify-center md:justify-start gap-3">
          <Icon name="lucide:instagram" size="23" class="text-red-500/90 hover:scale-110 cursor-pointer" />
          <Icon name="simple-icons:whatsapp" size="23" class="text-red-500/90 hover:scale-110 cursor-pointer" />
          <Icon name="lucide:mail" size="23" class="text-red-500/90 hover:scale-110 cursor-pointer" />
          <Icon name="lucide:phone" size="23" class="text-red-500/90 hover:scale-110 cursor-pointer" />
        </div>
      </div>

      <div class="flex flex-row md:justify-between md:w-2/3 gap-10 md:gap-20 text-center md:text-left">
        
        <div class="flex flex-col gap-3">
          <h3 class="font-bold text-xl">Links</h3>
          <ul class="text-gray-300 flex flex-col text-sm gap-1">
            <li>Início</li>
            <li>Sobre Nós</li>
            <li>Espaços</li>
            <li>Contato</li>
            <li>Localização</li>
          </ul>
        </div>

        <div class="flex flex-col gap-3">
          <h3 class="font-bold text-xl">Serviços</h3>
          <ul class="flex flex-col gap-1 text-gray-300 text-sm">
            <li>Musculação</li>
            <li>Treinamento Funcional</li>
            <li>Fit Dance</li>
            <li>CrossFit</li>
          </ul>
        </div>

        <div class="flex flex-col gap-3">
          <h3 class="font-bold text-xl">Endereço</h3>
          <p class="text-sm">
            Rua Exemplo, 123<br />
            Bairro, Cidade - Estado
          </p>
        </div>

      </div>
    </div>

    <hr class="w-full border-t border-gray-700" />

    <div class="flex flex-col md:flex-row justify-between items-center gap-3">
      <p class="text-center md:text-left text-sm text-gray-400">© 2024 GR FIT Academia. Todos os direitos reservados.</p>
      <p class="text-center md:text-left text-sm text-gray-400">Feito por <a href="">Ramon Kelvin</a></p>
    </div>
  </footer>
</template>
