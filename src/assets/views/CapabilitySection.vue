<template>
  <div
    class="w-full px-6 pt-10 mx-auto xl:pt-8 max-w-7xl pb-18 xl:pb-20 xl:px-0"
  >
    <h1
      data-aos-duration="1000"
      data-aos-once="false"
      data-aos="fade-up-left"
      class="text-base font-semibold leading-relaxed md:text-2xl capability-title xl:text-7xl"
    >
      CAPABILITIES
    </h1>

    <div class="pt-6 xl:pt-11" @click="isShowStrategy === false">
      <h6
        data-aos-easing="ease-out-cubic"
        data-aos-duration="1000"
        data-aos="flip-up"
        class="flex items-center text-base font-normal cursor-pointer hover:text-yellow-400 xl:text-2xl"
        @click="isShowStrategy = !isShowStrategy"
      >
        <span class="pr-2 text-lg font-normal" v-if="!isShowStrategy"> + </span>
        <span class="pr-2 text-lg font-normal" v-if="isShowStrategy"> - </span>
        Strategy
      </h6>

      <Transition name="slide">
        <div class="mt-4" v-if="isShowStrategy">
          <ul class="items-center xl:flex xl:space-x-8">
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Experience Design
              <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Branding <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Communicaton <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Packaging <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Retail
            </li>
          </ul>
        </div>
      </Transition>
    </div>

    <div class="pt-8" @click="isShowDesign === false">
      <h6
        data-aos-easing="ease-out-cubic"
        data-aos-duration="1000"
        data-aos="flip-down"
        class="flex items-center text-base font-normal cursor-pointer hover:text-yellow-400 xl:text-2xl"
        @click="isShowDesign = !isShowDesign"
      >
        <span class="pr-2 text-lg font-normal" v-if="!isShowDesign"> + </span>
        <span class="pr-2 text-lg font-normal" v-if="isShowDesign"> - </span>
        Design
      </h6>

      <Transition name="slide">
        <div class="mt-4" v-if="isShowDesign">
          <ul class="items-center xl:flex xl:space-x-8">
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Experience Design
              <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Branding <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Communicaton <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Packaging <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Retail
            </li>
          </ul>
        </div>
      </Transition>
    </div>

    <div class="pt-8">
      <h6
        data-aos-easing="ease-out-cubic"
        data-aos-duration="1000"
        data-aos="flip-up"
        class="flex items-center text-base font-normal cursor-pointer hover:text-yellow-400 xl:text-2xl"
        @click="isShowDigital = !isShowDigital"
      >
        <span class="pr-2 text-lg font-normal" v-if="!isShowDigital"> + </span>
        <span class="pr-2 text-lg font-normal" v-if="isShowDigital"> - </span>
        Digital
      </h6>

      <Transition name="slide">
        <div class="mt-4" v-if="isShowDigital">
          <ul class="items-center xl:flex xl:space-x-8">
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Experience Design
              <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Branding <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Communicaton <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Packaging <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Retail
            </li>
          </ul>
        </div>
      </Transition>
    </div>

    <div class="pt-8">
      <h6
        data-aos-easing="ease-out-cubic"
        data-aos-duration="1000"
        data-aos="flip-down"
        class="flex items-center text-base font-normal cursor-pointer hover:text-yellow-400 xl:text-2xl"
        @click="isShowMarketing = !isShowMarketing"
      >
        <span class="pr-2 text-lg font-normal" v-if="!isShowMarketing">
          +
        </span>
        <span class="pr-2 text-lg font-normal" v-if="isShowMarketing"> - </span>
        Marketing
      </h6>

      <Transition name="slide">
        <div class="mt-4" v-if="isShowMarketing">
          <ul class="items-center xl:flex xl:space-x-8">
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Experience Design
              <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Branding <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Communicaton <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Packaging <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Retail
            </li>
          </ul>
        </div>
      </Transition>
    </div>

    <div class="pt-8 pb-8">
      <h6
        data-aos-easing="ease-out-cubic"
        data-aos-duration="1000"
        data-aos="flip-up"
        class="flex items-center text-base font-normal cursor-pointer hover:text-yellow-400 xl:text-2xl"
        @click="isShowContentProduction = !isShowContentProduction"
      >
        <span class="pr-2 text-lg font-normal" v-if="!isShowContentProduction">
          +
        </span>
        <span class="pr-2 text-lg font-normal" v-if="isShowContentProduction">
          -
        </span>
        Content Production
      </h6>

      <Transition name="slide">
        <div class="mt-4" v-if="isShowContentProduction">
          <ul class="items-center xl:flex xl:space-x-8">
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Experience Design
              <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Branding <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Communicaton <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Packaging <span class="hidden pl-8 pr-6 xl:block"> | </span>
            </li>
            <li
              class="flex items-center mb-6 text-xs font-normal cursor-pointer xl:text-base hover:text-yellow-400"
            >
              Retail
            </li>
          </ul>
        </div>
      </Transition>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
let isShowStrategy = ref(false)
let isShowDesign = ref(false)
let isShowDigital = ref(false)
let isShowMarketing = ref(false)
let isShowContentProduction = ref(false)
</script>

<style scoped>
.capability-title {
  color: #fdcb03;
  /* font-family: Font Poppins; */
}

.slide-enter-active {
  transition: all 0.6s;
  opacity: 1;
  transform: translateY(5px);
}

.slide-leave-active {
  transition: all 0.2s;
  opacity: 1;
}

.slide-enter-from,
.slide-leave-to {
  transform: translateY(-5px);
  opacity: 0;
  transition: all 0.2s ease-out;
}
</style>
