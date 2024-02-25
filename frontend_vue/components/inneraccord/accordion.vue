<template>
  <div class="accordion w-full flex flex-col">
    <div class="py-2 w-full">
      <div class="flex w-full h-[40px] items-center gap-2 p-[2px] text-black text-[14px] hover:cursor-pointer"
        @click="toggle">
        <span>{{ title }}</span>
      </div>
      <div class="w-full relative transition-all px-2 duration-200 border bg-white rounded-md border-[#ccc] p-3"
        v-show="initialOpen">
        <div class="w-4 h-4 left-6 bg-white absolute z-[-1] border-[#ccc] border rotate-45 top-[-5px]"></div>
        <div class="w-4 h-4 left-6 bg-white absolute z-[0] rotate-45 top-[-4px]"></div>
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script setup>

const { title, initialOpen, index } = defineProps(['title', 'initialOpen', 'index'])
const emit = defineEmits(['toggle'])

const toggle = () => {
  emit('toggle');
};

</script>

