<template>
  <nav class="relative navbar navbar-inverse">
    <div class="">
      <!-- Site Logo and Menu Icon -->
      <div class="absolute top-0 left-0 right-0 mx-auto max-w-7xl">
        <div
          class="flex items-center justify-between px-4 pt-4 xl:px-12 xl:pt-8"
        >
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
    </div>

    <!-- Menu Item Container Overlay -->
  </nav>
  <transition name="slide">
    <div class="top-0 h-full overflow-hidden menu-overlay" v-if="isMobileMenu">
      <div class="z-50 overlay-menu-content">
        <div class="flex items-center justify-end px-4 pt-4 xl:px-12 xl:pt-8">
          <div class="flex justify-end">
            <button
              data-aos-duration="2000"
              data-aos="zoom-in-up"
              @click="isMobileMenu = !isMobileMenu"
              class="-mt-2 transition-all duration-500 ease-in-out transform hover:shadow-2xl"
            >
              <HumburgerIcon
                class="w-10 h-10 text-yellow-400 transition-all duration-500 bg-black rounded-full cursor-pointer xl:w-auto xl:h-auto hover:bg-black hover:rounded-full transform-gpu"
                v-if="!isMobileMenu"
              />
              <XIcon
                v-else
                class="w-10 h-10 p-1 text-yellow-400 transition-all duration-700 bg-black rounded-full cursor-pointer hover:rotate-180 xl:w-14 xl:h-14"
              />
            </button>
          </div>
        </div>

        <!-- Menu items content -->
        <header>
          <div class="flex items-center justify-center px-10 py-40 xl:px-20">
            <div class="py-40 xl:py-0 xl:mt-20">
              <ul class="p-0 pt-0 list-none xl:space-y-6 topBotomBordersOut">
                <li
                  data-aos="zoom-in-right"
                  data-aos-duration="3000"
                  class="flex items-center justify-center py-2 text-4xl font-bold text-center text-black transition-all duration-500 ease-in cursor-pointer hover:text-indigo-600 xl:text-6xl"
                >
                  Services
                </li>
                <li
                  data-aos="zoom-in-left"
                  data-aos-duration="3000"
                  class="flex items-center justify-center py-2 text-4xl font-bold text-center text-black transition-all duration-500 ease-in cursor-pointer hover:text-indigo-600 xl:text-6xl"
                >
                  Our Work
                </li>

                <li
                  data-aos="zoom-in-left"
                  data-aos-duration="3000"
                  class="flex items-center justify-center py-2 text-4xl font-bold text-center text-black transition-all duration-500 ease-in cursor-pointer hover:text-indigo-600 xl:text-6xl"
                >
                  About Us
                </li>
                <li
                  data-aos="zoom-in-right"
                  data-aos-duration="3000"
                  class="flex items-center justify-center py-2 text-4xl font-bold text-center text-black transition-all duration-500 ease-in cursor-pointer hover:text-indigo-600 xl:text-6xl"
                >
                  Resources
                </li>
              </ul>
            </div>
          </div>
        </header>
      </div>
    </div>
  </transition>
</template>

<script>
import SiteLogo from './icons/SiteLogo.vue'
import HumburgerIcon from './icons/HumburgerIcon.vue'
import { XIcon } from '@heroicons/vue/outline'
import AOS from 'aos'
export default {
  components: { SiteLogo, HumburgerIcon, XIcon },

  data() {
    return {
      isShow: false,
      isMobileMenu: false,
    }
  },

  methods: {},

  mounted() {
    $(window).scroll(function () {
      if ($(document).scrollTop() > 200) {
        $('nav').addClass('transparent ')
      } else {
        $('nav').removeClass('transparent')
      }
    })
    AOS.init()
  },
}
</script>

<style scoped>
nav.navbar {
  -webkit-transition: all 0.4s ease;
  animation-duration: 500ms;
  transition: all 0.9s ease;
  top: 0;
}

.navbar-inverse {
  animation-duration: 500ms;
  /* transform: translateY(10px); */
}

nav.navbar.transparent {
  position: fixed;
  z-index: 100;
  width: 100%;
  transition: width 6s all 0.5 ease;
  animation-duration: 400ms;
  height: 100px;
  transform: translateY(-20px);
  box-shadow: -10px 1px 9px 0px grey;
  background-color: white;
}

.navbar {
  padding: 0;
}
.menu-overlay {
  height: 100vh;
  width: 100%;
  position: fixed;
  z-index: 900;
  top: 0;
  left: 0;
  background-color: #fdcb03;
  overflow-x: hidden;
}

.overlay-menu-content {
  position: relative;
  width: 100%;
  text-align: center;
}

.cover-img {
  height: 100%;
}

.slide-enter-active {
  transform: translateX(2000);
  opacity: 1;
  transition: all 0.9s ease-in-out;
}

.slide-leave-active {
  transition: all 0.9s ease;
  opacity: 1;
}

.slide-enter-from,
.slide-leave-to {
  transform: translateX(2000px);
  opacity: 0;
  transition: all 0.5s ease-in-out;
}

/* * Navbar Item Top and Bottom borders go out */
ul.topBotomBordersOut li:before,
ul.topBotomBordersOut li:after {
  position: absolute;
  left: 0px;
  right: 0px;
  width: 100%;
  display: flex;
  text-align: center;
  justify-content: center;
  height: 2px;
  background: white;
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
