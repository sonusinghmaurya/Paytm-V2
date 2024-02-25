<script setup>


const img = ref('https://pwebassets.paytm.com/commonwebassets/paytmweb/header/images/loginImg.svg')
const SideMenuBtn = ref(false)
const DropComp = ref(false)
const DropCompBtn = ref(false)
const DropInvBtn = ref(false)
const DropCarBtn = ref(false)

const changeSigninLogoImg = () => {
  img.value = 'https://pwebassets.paytm.com/commonwebassets/paytmweb/header/images/logoutImg.svg';
};

const leaveSigninLogo = () => {
  img.value = 'https://pwebassets.paytm.com/commonwebassets/paytmweb/header/images/loginImg.svg'
}

const DropDown = () => {
  DropComp.value = !DropComp.value
  DropCompBtn.value = true
}

const ClickEdLinkInv = () => {
  DropInvBtn.value = true

  if (DropInvBtn.value == true) {
    setTimeout(() => {
      DropInvBtn.value = false;
    }, 400);
  }

}

const ClickEdLinkCar = () => {
  DropCarBtn.value = true

  if (DropCarBtn.value == true) {
    setTimeout(() => {
      DropCarBtn.value = false;
    }, 400);
  }
}

onUpdated(() => {
  if (DropCompBtn.value == true) {
    setTimeout(() => {
      DropCompBtn.value = false;
    }, 400);
  }
})

const OpenSideMenu = () => {
  SideMenuBtn.value = !SideMenuBtn.value
}

const HomePage = () => {
  navigateTo('/')
  OpenSideMenu()
}
</script>

<template>
  <div class="w-full">
    <div
      class="fixed z-50 left-0 top-0 h-lvh overflow-hidden transition-all duration-300 bg-white flex flex-col lg:hidden"
      :class="{ 'w-full': SideMenuBtn, 'w-0': !SideMenuBtn }">
      <div class="flex justify-start items-center h-16 gap-6 px-[20px] shadow-lg z-50 w-full">
        <i class="material-icons cursor-pointer" @click="OpenSideMenu">close</i>
        <img class="w-32 transition-transform duration-300 lg:w-[180px] cursor-pointer" @click="HomePage"
          src="/assets/images/logo.svg" alt="">
      </div>
      <div class="flex flex-col justify-start p-[18px] text-[20px] font-semibold text-nowrap h-screen bg-[#fafafa]">
        <div
          class="relative w-full flex justify-between items-center  cursor-pointer border-t border-b border-gray-200 py-7"
          @click="ClickEdLinkInv">
          <nuxt-link to="/">Investor Relations</nuxt-link>
          <i class="material-icons text-gray-500">
            chevron_right
          </i>
          <div
            class="absolute h-full blur-[1px] top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] transition-all"
            :class="{ 'w-full BackGradient': DropInvBtn, 'w-0': !DropInvBtn }"></div>
        </div>
        <div class="w-full flex justify-between flex-col items-center  cursor-pointer">
          <div
            class="w-full flex justify-between items-center cursor-pointer border-t border-b border-gray-200 py-7 relative"
            @click="DropDown">
            <nuxt-link to="/" :class="{ 'text-black': !DropComp, 'text-[#00baf2]': DropComp }">Company</nuxt-link>
            <i class="material-icons text-gray-500">
              {{ DropComp ? 'expand_less' : 'expand_more' }}
            </i>
            <div
              class="absolute h-full blur-[1px] top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] transition-all"
              :class="{ 'w-full BackGradient': DropCompBtn, 'w-0': !DropCompBtn }"></div>
          </div>
          <div class="overflow-hidden w-full transition-all duration-100 text-[16px] bg-white text-gray-600"
            :class="{ 'h-full mt-3 space-y-7 py-5': DropComp, 'h-0 mt-0 p-0': !DropComp }">
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">About</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">CSR</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">Blog</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">Contact Us</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">Terms & Conditions</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
            <div class="w-full flex justify-between items-center  cursor-pointer">
              <nuxt-link to="/">Sustainability</nuxt-link>
              <i class="material-icons text-gray-500">
                chevron_right
              </i>
            </div>
          </div>
        </div>
        <div
          class="relative w-full flex justify-between items-center  cursor-pointer border-t border-b border-gray-200 py-7"
          @click="ClickEdLinkCar">
          <nuxt-link to="/">Career</nuxt-link>
          <i class="material-icons text-gray-500">
            chevron_right
          </i>
          <div
            class="absolute h-full blur-[1px] top-[50%] left-[50%] translate-x-[-50%] translate-y-[-50%] transition-all"
            :class="{ 'w-full BackGradient': DropCarBtn, 'w-0': !DropCarBtn }"></div>
        </div>
      </div>
    </div>
    <header
      class="fixed z-40 top-0 left-0 w-full flex justify-between items-center lg:px-[10px] px-[20px] py-[9px] bg-white shadow-lg xl:px-[120px] 2xl:px-[226px]">
      <div class="flex justify-center items-center gap-3">
        <i class="material-icons lg:hidden cursor-pointer" @click="OpenSideMenu">menu</i>
        <img class="w-32 transition-transform duration-300 lg:w-[180px] cursor-pointer" @click="navigateTo('/')"
          src="/assets/images/logo.svg" alt="">
      </div>
      <ul class="hidden lg:flex justify-center items-center gap-4 text-[15px] font-bold xl:gap-8 text-nowrap">
        <li>
          <nuxt-link to="/">Paytm for Consumer</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">Paytm For Bussiness</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">Investor Realtions</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">Company</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/">Career</nuxt-link>
        </li>
      </ul>
      <div @mouseenter="changeSigninLogoImg" @mouseleave="leaveSigninLogo"
        class="flex justify-center items-center gap-4 bg-[#00baf2] hover:bg-[#002970] transition-all duration-200 cursor-pointer text-white p-[6px] rounded-3xl"
        @click="navigateTo('/login')">
        <p class="ml-[8px] text-nowrap">Sign in</p>
        <img :src="img" alt="">
      </div>
    </header>
    <div class="mt-[75px] flex justify-start flex-col">
      <div class="z-30">
        <marquee
          class="capitalize bg-yellow-300 p-2 text-center text-white font-bold tracking-widest text-lg"
          behavior="smooth" direction="left">
          <icon name="mingcute:alert-fill" />
          This website-clone is for learing purposes only
        </marquee>
      </div>
      <slot />
    </div>
    <div
      class="fixed bottom-0 left-0 z-40 w-full flex justify-between items-center bg-[#e8f8fd] px-[20px] py-[15px] lg:hidden">
      <div class="flex justify-center items-center gap-3">
        <img class="w-[40px]" src="/assets/images/mobiledownload/paytmLogo.svg" alt="">
        <div>
          <p class="font-bold text-xs text-[#4f4f4f]">Download the App</p>
          <p class="font-medium text-xs text-black">Live the paytm Experience</p>
        </div>
      </div>
      <nuxt-link
        class="px-[15px] py-[10px] text-xs text-white transition-all duration-200 bg-[#00baf2] rounded-3xl font-semibold tracking-wide hover:bg-white hover:text-[#00baf2] border hover:border-[#00baf2]"
        to="/">Download Now</nuxt-link>
    </div>
  </div>
</template>

<style scoped>
.BackGradient {
  transition: all 0.3s ease;
  background: linear-gradient(to left, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.2));
  ;
}

.BackGradient:after {
  display: none;
}</style>