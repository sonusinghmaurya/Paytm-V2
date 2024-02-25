<template>
  <div
    class="flex justify-between items-center flex-col bg-[#00baf2] rounded-lg p-2 w-[160px] h-[240px] transition-all duration-200 opacity-50 hover:opacity-100 cursor-pointer"
    @click="navigateTo('/')">
    <div class="overflow-hidden group rounded-lg">
      <img class="group-hover:scale-110 transition-all duration-200"
        :src="image" alt="">
    </div>
    <div class="h-[60px] flex justify-center items-center px-[20px]">
      <p class="text-white text-[18px] font-semibold text-center">{{ text }}</p>
    </div>
  </div>
</template>

<script setup>
const { image, text } = defineProps(['image', 'text'])

console.log(image, text);
</script>