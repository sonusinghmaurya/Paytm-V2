<script setup>

const { name, device, image } = defineProps(['name','device', 'image'])

</script>

<template>
  <div class="flex flex-col justify-center text-white min-w-32 max-w-36 cursor-pointer gap-1 hover:bg-[#0f3e8a] p-4 rounded-lg hover:shadow-sm">
    <img class="w-[44px] md:w-[64px]" :src="image" alt="">
    <p class="text-[16px] font-semibold tracking-wide
    mt-4">{{ name }}</p>
    <div class="flex flex-col text-[14px] tracking-wider">
      <p class="">
        <span>{{ device }}</span>
        <Icon name="fluent:ios-arrow-right-24-filled" />
      </p>
    </div>
  </div>
</template>