<template>
  <div class="flex flex-col justify-between w-full h-[500px] items-left">
    <div>
      <div class="flex justify-center items-center mb-8">
        <img class="w-[250px]" :src="image"
          alt="">
      </div>
      <h1 class="text-[24px] font-bold tracking-wide flex flex-col">
        <span>
          {{ headtext1 }}
        </span>
        <span>
          {{ headtext2 }}
        </span>
      </h1>
      <p class="text-[17px] my-[10px]">
        {{ para }}
      </p>
    </div>
    <nuxt-link class="flex justify-start items-center gap-1 relative text-black text-[16px] group hover:text-[#00baf2] transition-all duration-300" to="/">
      <div>
        Learn More
      </div>
      <div class="relative w-[20px] h-full overflow-hidden text-black">
        <Icon
          class="text-[16px] transition-all duration-300 absolute top-[50%] left-[-50%] translate-x-[-50%] translate-y-[-50%] group-hover:left-[50%] group-hover:text-[#00baf2]"
          name="tabler:arrow-right" />
      </div>
    </nuxt-link>
  </div>
</template>

<script setup>

const { headtext1, headtext2, image, para, } = defineProps(['headtext1', 'headtext2', 'image', 'para'])

</script>