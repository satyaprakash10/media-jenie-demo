<template>
  <div class="relative">
    <!-- Site Main header  -->
    <div>
      <img
        src="../assets/images/site-cover-img.png"
        class="hidden w-full xl:block"
        alt=""
      />
      <img
        src="../assets/images/site-cover-img.png"
        class="block w-full bg-cover xl:hidden"
        style="height: 400px"
        alt=""
      />

      <div class="absolute inset-0 top-48 md:top- xl:top-1/2">
        <h1
          data-aos="zoom-in"
          data-aos-duration="1000"
          data-aos-delay="50"
          data-aos-easing="ease-in-out"
          class="text-xl font-semibold text-center text-white sm:text-2xl xl:text-5xl"
        >
          5 Vaishnavi Estate
        </h1>
        <h6
          data-aos="fade-up"
          data-aos-duration="1000"
          class="mt-3 text-base font-semibold text-center text-white xl:text-xl"
        >
          Content Production
        </h6>
      </div>
    </div>

    <!-- Site Logo and Menu Icon -->
    <div class="absolute top-0 left-0 right-0 xl:px-8">
      <div class="flex items-center justify-between px-4 pt-4 xl:px-12 xl:pt-8">
        <div data-aos="fade-right" data-aos-duration="1000">
          <SiteLogo />
        </div>
        <div
          class="flex justify-end"
          data-aos="fade-left"
          data-aos-duration="1000"
        >
          <button @click="isMobileMenu = !isMobileMenu" class="">
            <HumburgerIcon
              class="transition-all ease-in-out rounded-full shadow-lg cursor-pointer duration-900 hover:shadow-2xl"
              v-if="!isMobileMenu"
            />
            <XIcon
              v-else
              class="p-1 transition-all duration-1000 bg-yellow-400 rounded-full cursor-pointer hover:rotate-180 w-14 h-14"
            />
          </button>
        </div>
      </div>
    </div>

    <!-- Menu Item Container Overlay -->
    <transition name="slide">
      <div class="top-0 z-40 menu-overlay" v-if="isMobileMenu">
        <div class="overlay-menu-content">
          <div
            class="flex items-center justify-between px-4 pt-4 xl:px-12 xl:pt-8"
          >
            <div class="cursor-pointer">
              <SiteLogo
                class="w-8 h-8 text-white xl:w-auto xl:h-auto"
                data-aos="fade-down"
                data-aos-duration="2000"
              />
              <div
                data-aos="fade-up"
                data-aos-duration="2000"
                class="px-3 font-sans text-base font-bold text-white xl:-mt-2 hover:text-yellow-400 xl:text-2xl"
              >
                Media Jenie
              </div>
            </div>

            <div class="flex justify-end">
              <button
                data-aos-duration="2000"
                data-aos="zoom-in-up"
                @click="isMobileMenu = !isMobileMenu"
                class="-mt-2 transition-all duration-500 ease-in-out transform hover:shadow-2xl"
              >
                <HumburgerIcon
                  class="w-10 h-10 transition-all duration-500 rounded-full cursor-pointer xl:w-auto xl:h-auto hover:bg-yellow-600 hover:rounded-full transform-gpu"
                  v-if="!isMobileMenu"
                />
                <XIcon
                  v-else
                  class="w-10 h-10 p-1 transition-all duration-700 bg-yellow-400 rounded-full cursor-pointer hover:rotate-180 xl:w-14 xl:h-14"
                />
              </button>
            </div>
          </div>
          <!-- Menu items content -->
          <header>
            <div class="px-10 py-10 xl:px-20 xl:py-20">
              <h1
                data-aos="zoom-in-right"
                data-aos-duration="2000"
                class="flex items-center justify-center text-xl font-bold leading-relaxed text-center text-yellow-400 xl:justify-end xl:text-right md:text-2xl xl:text-5xl"
              >
                Media Jenie |
                <span
                  data-aos="fade-left"
                  data-aos-duration="1000"
                  class="text-base font-bold text-white md:text-xl xl:text-3xl"
                >
                  Digital Media Agency
                </span>
              </h1>
              <div class="mt-10 xl:mt-20">
                <ul class="p-0 pt-0 space-y-10 list-none topBotomBordersOut">
                  <li
                    data-aos="zoom-in-right"
                    data-aos-duration="2000"
                    class="py-4 text-xl font-bold text-center text-white transition-all duration-500 ease-in cursor-pointer xl:w-96 xl:text-left md:text-xl xl:text-5xl hover:text-yellow-400"
                  >
                    Home
                  </li>
                  <li
                    data-aos="zoom-in-left"
                    data-aos-duration="2000"
                    class="py-4 text-xl font-bold text-center text-white transition-all duration-500 ease-in cursor-pointer xl:w-96 xl:text-left md:text-xl xl:text-5xl hover:text-yellow-400"
                  >
                    About
                  </li>
                  <li
                    data-aos="zoom-in-right"
                    data-aos-duration="2000"
                    class="py-4 text-xl font-bold text-center text-white transition-all duration-500 ease-in cursor-pointer xl:w-96 xl:text-left md:text-xl xl:text-5xl hover:text-yellow-400"
                  >
                    Portfolio
                  </li>
                  <li
                    data-aos="zoom-in-left"
                    data-aos-duration="2000"
                    class="py-4 text-xl font-bold text-center text-white transition-all duration-500 ease-in cursor-pointer xl:w-96 xl:text-left md:text-xl xl:text-5xl hover:text-yellow-400"
                  >
                    Contact Us
                  </li>
                  <li
                    data-aos="zoom-in-right"
                    data-aos-duration="2000"
                    class="py-4 text-xl font-bold text-center text-white transition-all duration-500 ease-in cursor-pointer xl:w-96 xl:text-left md:text-xl xl:text-5xl hover:text-yellow-400"
                  >
                    Support
                  </li>
                </ul>
              </div>
            </div>
          </header>
        </div>
      </div>
    </transition>
  </div>
</template>

<script setup>
import SiteLogo from './icons/SiteLogo.vue'
import HumburgerIcon from './icons/HumburgerIcon.vue'
import { XIcon } from '@heroicons/vue/outline'
import { ref, onMounted } from 'vue'
import AOS from 'aos'

let isShow = ref(false)
let isMobileMenu = ref(false)

onMounted(() => {
  AOS.init()
})
</script>

<style scoped>
.menu-overlay {
  height: 100%;
  width: 100%;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: rgb(0, 0, 0);
  background-color: rgba(0, 0, 0, 0.9);
  overflow-x: hidden;
}

.overlay-menu-content {
  position: relative;
  width: 100%;
  text-align: center;
}

.cover-img {
  height: 606px;
}

.slide-enter-active {
  transform: translateY(-200);
  opacity: 1;
  transition: all 0.9s ease-in-out;
}

.slide-leave-active {
  transition: all 0.9s ease;
  opacity: 1;
}

.slide-enter-from,
.slide-leave-to {
  transform: translateY(-700px);
  opacity: 0;
  transition: all 0.5s ease-in-out;
}

/* * Navbar Item Top and Bottom borders go out */
ul.topBotomBordersOut li:before,
ul.topBotomBordersOut li:after {
  position: absolute;
  left: 0px;
  width: 100%;
  height: 2px;
  background: #fff;
  content: '';
  opacity: 0;
  transition: all 0.3s;
}

ul.topBotomBordersOut li:before {
  top: 0px;
  transform: translateY(10px);
}

ul.topBotomBordersOut li:after {
  bottom: 0px;
  transform: translateY(-10px);
}

ul.topBotomBordersOut li:hover:before,
ul.topBotomBordersOut li:hover:after {
  opacity: 1;
  transform: translateY(0px);
}
</style>
