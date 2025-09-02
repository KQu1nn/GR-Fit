<template>
    <div v-for="data in infosWorkCards" class="min-w-[360px] h-[230px] border-l-[8px] border-red-500 flex flex-row items-center justify-between text-black bg-gray-50 shadow-lg hover:shadow-2xl hover:scale-105 transition ease-in-out duration-300">
        <div class="w-[150px] h-[230px] ">
            <img :src="data.image" class="w-full h-full object-cover" />
        </div>
        <div class="w-[230px] flex flex-col flex-1 gap-3 py-2 px-3 ">
            <h2 class="text-2xl font-bold bg-gradient-to-r text-gray-900">{{ data.title }}</h2>
            <p class="text-sm text-start">{{ data.description }}</p>
        </div>
    </div>
</template>

<script setup>

defineProps({
  infosWorkCards: {
    type: Array,
    required: true
  }
})
</script>