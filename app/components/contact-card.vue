<template>
  <div class="w-[385px] h-[208px] rounded-lg pt-5 px-5 flex flex-col justify-center gap-3 bg-neutral-900/80 shadow-xl">
    <div class="flex items-center gap-3">
      <span class=" w-10 h-10 rounded-full bg-red-500 flex items-center justify-center">
        <Icon :name="dataContact.icon" size="24" class="text-white" />
      </span>
      <h4 class="text-xl font-bold">{{ dataContact.title }}</h4>
    </div>
    <div class="flex flex-col">
      <div class="flex flex-col gap-1">
        <span class="text-lg font-medium">{{ dataContact.description }}</span>
        <span class="text-sm text-gray-400">{{ dataContact.subdescription }}</span>
      </div>
      <a :href="dataContact.url" target="_blank" rel="noopener noreferrer">
        <button aria-labels="contato" class="bg-red-500/80 hover:scale-105 transition ease-in-out duration-200 text-white w-full my-5 py-2 rounded-lg cursor-pointer">{{ dataContact.button }}</button>
      </a>
    </div>

  </div>
</template>

<script setup>
defineProps({
  dataContact: {
    type: Object,
    required: true
  }
})
</script>
