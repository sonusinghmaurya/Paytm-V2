<template>
  <div
    class="flex justify-around items-center flex-col bg-[#00baf2] rounded-lg p-2 w-[160px] h-[240px] transition-all duration-200 opacity-50 hover:opacity-100 cursor-pointer"
    @click="navigateTo('/')">
    <div class="flex justify-center w-full group rounded-lg">
      <img class="w-[64px] group-hover:scale-110 transition-all duration-200" :src="image" alt="">
    </div>
    <div class="flex justify-center items-center px-[20px]">
      <p class="text-white text-[16px] font-semibold text-center">{{ text }}</p>
    </div>
  </div>
</template>

<script setup>
const { image, text } = defineProps(['image', 'text'])
</script>