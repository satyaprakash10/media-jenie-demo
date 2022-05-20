<template>
  <div class="relative w-full py-10 xl:max-w-7xl xl:mx-auto">
    <div class="flex justify-center">
      <div
        class="absolute -top-8"
        data-aos="zoom-out-up"
        data-aos-duration="900"
      >
        <button
          class="z-40 text-base font-semibold text-black transition-all duration-500 ease-in hover:bg-yellow-600 hover:shadow-xl button"
        >
          View more work
        </button>
      </div>
    </div>

    <div
      class="items-center justify-between px-6 mt-10 xl:flex xl:mt-20 xl:px-12"
    >
      <div>
        <h6
          data-aos="fade-down"
          data-aos-duration="1000"
          class="text-base font-semibold leading-relaxed xl:text-2xl feature-text"
        >
          CASE STUDY
        </h6>
        <p
          class="pt-6 text-xl font-semibold xl:text-3xl"
          data-aos="fade-right"
          data-aos-duration="1000"
        >
          How a US start-up generated 250K USD revenue in 1 year from website.
        </p>

        <div
          class="flex justify-center mt-4 pt-14 xl:justify-start"
          data-aos="fade-up"
          data-aos-duration="1000"
        >
          <button
            class="z-40 text-base font-semibold text-black transition-all duration-500 ease-in btn hover:bg-yellow-600 hover:shadow-xl"
          >
            Download
          </button>
        </div>
      </div>

      <div class="block mt-10 md:flex md:space-x-10 xl:hidden">
        <div class="">
          <img
            src="../../assets/images/work/work-web-04.png"
            class="w-full h-96"
            alt=""
            data-aos="fade-down"
            data-aos-easing="linear"
            data-aos-duration="1500"
          />
        </div>
        <div class="mt-6 md:mt-0">
          <img
            data-aos="fade-up"
            data-aos-easing="linear"
            data-aos-duration="1500"
            src="../../assets/images/work/work-web-05.png"
            class="w-full h-96"
            alt=""
          />
        </div>
      </div>

      <div class="gap-8 xl:flex">
        <div class="hidden xl:block">
          <img
            data-aos="fade-down"
            data-aos-easing="linear"
            data-aos-duration="1500"
            width="400"
            height="398"
            src="../../assets/images/work/work-web-04.png"
            class="w-full sm:auto"
            alt="Man"
          />
        </div>

        <div class="">
          <div class="hidden xl:block">
            <img
              data-aos="fade-up"
              data-aos-easing="linear"
              width="260"
              height="260"
              data-aos-duration="1500"
              src="../../assets/images/work/work-web-05.png"
              class=""
              alt="Women"
            />
          </div>
          <div class="mt-4">
            <h6
              data-aos="fade-down"
              data-aos-easing="linear"
              data-aos-duration="1000"
              class="text-base font-semibold leading-relaxed xl:text-xl feature-text"
            >
              ARTICLE
            </h6>
            <p
              class="pt-2 text-xl font-semibold xl:text-xl"
              data-aos="fade-up"
              data-aos-easing="linear"
              data-aos-duration="1000"
            >
              How a US start-up generated 250K USD revenue in 1 year from
              website.
            </p>

            <div
              class="mt-4"
              data-aos="fade-right"
              data-aos-easing="linear"
              data-aos-duration="1000"
            >
              <RightArrowIcon
                class="overflow-hidden transition-all duration-700 ease-in-out transform cursor-pointer hover:text-yellow-400 hover:scale-x-90"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import RightArrowIcon from '../../components/icons/RightArrowIcon.vue'
</script>

<style scoped>
.button {
  background: #fdcc06;
  color: #000000;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  width: 227px;
  height: 58px;
  transition: all 0.5s;
}

.button:before {
  width: 227px;
  height: 58px;
  content: '';
  margin: auto;
  position: absolute;
  top: -100%;
  left: -100%;
  background: #212121;
  transition: all 0.5s;
  z-index: -1;
}

.button:hover {
  color: white;
}

.button:hover:before {
  top: 0;
  left: 0;
}

.btn {
  background: #fdcc06;
  color: #000000;
  cursor: pointer;
  border-radius: 0px;
  position: relative;
  overflow: hidden;
  width: 159px;
  height: 58px;
  transition: all 0.5s;
}

.btn:before {
  width: 159px;
  height: 58px;
  content: '';
  margin: auto;
  position: absolute;
  top: -100%;
  left: -100%;
  background: #212121;
  transition: all 0.5s;
  z-index: -1;
}

.btn:hover {
  color: white;
}

.btn:hover:before {
  top: 0;
  left: 0;
}

.web-img {
  height: 398px;
}

.feature-text {
  color: #fdcb03;
}
</style>
