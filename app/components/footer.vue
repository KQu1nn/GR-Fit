<template>
  <div class="w-full px-20 py-10 bg-neutral-900 text-white flex flex-row items-center">
    <div class="w-1/2 flex flex-col gap-5">
      <div class=" flex flex-row gap-5 items-center cursor-pointer">
        <p class="font-sans italic text-xl  font-bold">GR FIT <span class="text-red-500">Academia</span></p>
      </div>
      <p class="text-gray-300 text-sm w-4/6">Mais que uma academia. Somos um espaço de acolhimento, força e evolução. Na
        GRFIT, cada treino tem um
        propósito. E cada pessoa é único.</p>
      <div>
        <Icon name="lucide:instagram" size="23" class="text-red-500/90 hover:scale-110 mr-3 cursor-pointer" />
        <Icon name="simple-icons:whatsapp" size="23" class="text-red-500/90 hover:scale-110 mr-3 cursor-pointer" />
        <Icon name="lucide:mail" size="23" class="text-red-500/90 hover:scale-110 mr-3 cursor-pointer" />
        <Icon name="lucide:phone" size="23" class="text-red-500/90 hover:scale-110 mr-3 cursor-pointer" />
      </div>
    </div>
    <div class="flex flex-row justify-around w-1/2">
      <div class="flex flex-col gap-3">
        <h3 class="font-bold text-xl ">Links</h3>
        <ul class="text-gray-300 flex flex-col  text-sm">
          <li>Início</li>
          <li>Sobre Nós</li>
          <li>Espaços</li>
          <li>Contato</li>
          <li>Localização</li>
        </ul>
      </div>
      <div class="flex flex-col gap-3">
        <h3 class="font-bold text-xl ">Serviços</h3>
        <ul class="flex flex-col gap-1">
          <li class="text-gray-300 text-sm">Musculação</li>
          <li class="text-gray-300 text-sm">Treinamento Funcional</li>
          <li class="text-gray-300 text-sm">Fit Dance</li>
          <li class="text-gray-300 text-sm">CrossFit</li>
        </ul>
      </div>
      <div class="flex flex-col gap-3">
        <h3 class="font-bold text-xl ">Endereço</h3>
        <p class="text-sm">Rua Exemplo, 123<br>
          Bairro, Cidade - Estado</p>
      </div>
    </div>
  </div>
</template>
