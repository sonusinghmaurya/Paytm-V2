<template>
<div :style="{ width: `${sliderWidth + 100}px` }" class="border border-black rounded-lg p-3">
  <div class="flex flex-col items-center gap-4">
    <h1 class="text-[25px] font-bold mb-10">{{ name }}</h1>
    <!-- <p class="text-2xl capitalize font-serif">percent : {{ parseInt(percentageX / multiplyer) * multiplyer }}%</p> -->
    <div @mousedown="clickButton" :style="{ width: `${sliderWidth}px` }" class="h-[5px] rounded-[35px] relative bg-green-300 my-5 silder_outter_div">
      <div class="w-[35px] h-[15px] rounded-full shadow-2xl top-[50%] translate-y-[-50%] absolute bg-red-400 slider_button cursor-pointer" :style="{ left: `${posX}px` }">
        <div class="absolute z-20 w-12 h-12 rounded-full flex justify-center items-center bg-blue-500 top-[-55px] left-[50%] translate-x-[-50%] shadow-2xl">
          <div class="absolute bg-blue-500 z-30 w-5 h-5 rotate-45 top-7 left-[50%] translate-x-[-50%] shadow-2xl"></div>
          <p class="text-white z-50 font-sans text-[18px]">{{ parseInt(percentageX / multiplyer) * multiplyer }} </p>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
const {
  sliderWidth,
  name,
  multiplyer
} = defineProps(['sliderWidth', 'name', 'multiplyer']);

const offsetX = ref(0)
const posX = ref(0)
const percentageX = ref(0);

const clickButton = (e) => {
  offsetX.value = e.clientX - e.target.getBoundingClientRect().left
  document.addEventListener('mousemove', dragButton)
  document.addEventListener('mouseup', saveBtnPos)
}

const dragButton = (e) => {
  const newX = e.clientX - offsetX.value - document.querySelector('.silder_outter_div').getBoundingClientRect().left;
  const minPosX = 0
  const maxPosX = document.querySelector('.silder_outter_div').clientWidth - document.querySelector('.slider_button').clientWidth;
  posX.value = Math.max(minPosX, Math.min(maxPosX, newX))

  // Calculate percentage
  const percentage = (posX.value / maxPosX) * 100;
  percentageX.value = Math.round(percentage);
}

const saveBtnPos = () => {
  document.removeEventListener('mousemove', dragButton);
  document.removeEventListener('mouseup', saveBtnPos);
}

onMounted(() => {
  const maxPositionX = document.querySelector('.silder_outter_div').clientWidth - document.querySelector('.slider_button').clientWidth;
  const percentage = (posX.value / maxPositionX) * 100;
  percentageX.value = Math.round(percentage);
});
</script>
