<script setup>

const { name, type, device, image } = defineProps(['name', 'type', 'device', 'image'])

</script>

<template>
  <div class="flex flex-col justify-center text-white min-w-32 max-w-36 cursor-pointer gap-1 hover:bg-[#00c2f2] p-4 rounded-lg hover:shadow-sm transition-all duration-300">
    <img class="w-[44px] md:w-[64px] " :src="image" alt="">
    <p class="text-[16px] font-semibold tracking-wide
    mt-4">{{ name }}</p>
    <div class="flex flex-col text-[14px] tracking-wider">
      <p>{{ type }}</p>
      <p class="">
        <span>{{ device }}</span>
        <Icon name="fluent:ios-arrow-right-24-filled" />
      </p>
    </div>
  </div>
</template>

<!-- <style scoped>
  .custom_cursor {
    cursor: url('https://img.icons8.com/material-rounded/24/movie-projector.png'), auto;
  }
</style> -->