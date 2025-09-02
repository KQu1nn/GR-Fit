<template>
    <div v-for="data in infosWorkCards" class="min-w-[320px] h-[250px] border-l-[8px] border-red-500 flex flex-row items-center text-black bg-gray-50 shadow-lg hover:shadow-2xl hover:scale-105 transition ease-in-out duration-300">
        <div class="w-[170px] h-[250px] ">
            <img :src="data.image" class="w-[170px] h-[250px] object-cover " />
        </div>
        <div class=" flex flex-col flex-1 gap-3 p-5 ">
            <h2 class="text-3xl font-bold bg-gradient-to-r text-gray-900">{{ data.title }}</h2>
            <p class="font-sm text-start">{{ data.description }}</p>
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