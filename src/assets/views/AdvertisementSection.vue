<template>
  <div class="w-full border-gray-300 border-b-1">
    <!-- Site Main header  -->
    <div class="">
      <img
        src="../../assets/images/site-cover-img.png"
        class="hidden w-full bg-center bg-no-repeat bg-cover xl:block"
        alt=""
        style="height: 645px"
      />
      <img
        src="../../assets/images/site-cover-img.png"
        class="block w-full bg-contain xl:hidden"
        style="height: 400px"
        alt=""
      />

      <div class="absolute inset-0 top-40 xl:top-72">
        <h1
          data-aos="zoom-in"
          data-aos-duration="1000"
          data-aos-delay="50"
          data-aos-easing="ease-in-out"
          class="text-3xl font-semibold text-center text-white sm:text-2xl xl:text-5xl"
        >
          5 Vaishnavi Estate
        </h1>
        <h6
          data-aos="fade-up"
          data-aos-duration="1000"
          class="mt-3 text-xl font-semibold text-center text-white xl:text-xl"
        >
          Content Production
        </h6>
      </div>
    </div>
    <div class="pt-4 pb-4 xl:pb-7">
      <div class="mx-auto max-w-7xl">
        <div class="items-center mx-auto md:px-6 max-w-7xl md:flex">
          <h3
            class="flex justify-center hidden font-medium text-gray-900 xl:font-normal md:justify-start xl:block md:block lg:block xl:text-xl"
            data-aos-duration="1000"
            data-aos="zoom-in-right"
          >
            TRUSTED BY
          </h3>

          <div class="w-full xl:mx-auto xl:max-w-7xl">
            <div class="hidden md:block sm:hidden xl:block lg:block">
              <div
                class="flex items-center justify-center w-full space-x-10 xl:space-x-24"
              >
                <div
                  data-aos-duration="1000"
                  data-aos-once="true"
                  data-aos="zoom-out-right"
                >
                  <img
                    src="../../assets/images/advertisement/apple-adv.png"
                    width="118px"
                    height="118px"
                    class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-110"
                    alt=""
                  />
                </div>
                <div
                  data-aos-duration="1000"
                  data-aos-once="true"
                  data-aos="zoom-in-up"
                >
                  <img
                    src="../../assets/images/advertisement/gloria-jeans-adv.png"
                    alt=""
                    width="118px"
                    class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-110"
                    height="118px"
                  />
                </div>
                <div
                  data-aos-duration="1000"
                  data-aos-once="true"
                  data-aos="zoom-in-up"
                >
                  <img
                    src="../../assets/images/advertisement/happilo-adv.png"
                    alt=""
                    class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-110"
                    width="98px"
                    height="45px"
                  />
                </div>
                <div
                  data-aos-duration="1000"
                  data-aos-once="true"
                  data-aos="zoom-in-up"
                >
                  <img
                    src="../../assets/images/advertisement/hsc-adv.png"
                    alt=""
                    class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-110"
                    width="70px"
                    height="70px"
                  />
                </div>
                <div
                  data-aos-duration="1000"
                  data-aos-once="true"
                  data-aos="zoom-in-left"
                >
                  <img
                    src="../../assets/images/advertisement/toyoda-adv.png"
                    alt=""
                    class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-110"
                    width="164px"
                    height="68px"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Mobile advertisement Slider  -->
    <div class="relative">
      <div
        class="absolute inset-0 block w-full h-40 mx-auto bg-yellow-400 md:hidden md:-top-60 bg-opacity-90 -top-32 max-w-7xl sm:block xl:hidden"
      >
        <div
          id="carouselExampleControls"
          class="w-full carousel slide"
          data-ride="carousel"
        >
          <div class="carousel-inner">
            <div class="h-40 carousel-item active">
              <img
                class="flex items-center w-40 h-full mx-auto d-block max-w-7xl"
                src="../../assets/images/advertisement/apple-adv.png"
                alt="Appple Advertisement"
              />
            </div>
            <div class="h-40 carousel-item">
              <img
                class="flex items-center w-40 h-full mx-auto d-block max-w-7xl"
                src="../../assets/images/advertisement/gloria-jeans-adv.png"
                alt="Gloria Jeans Advertisement"
              />
            </div>
            <div class="h-40 carousel-item">
              <img
                class="flex items-center w-40 h-auto mx-auto mt-10 d-block max-w-7xl"
                src="../../assets/images/advertisement/happilo-adv.png"
                alt="Happilo Advertisement"
              />
            </div>
            <div class="h-40 carousel-item">
              <img
                class="flex items-center w-40 h-full mx-auto d-block max-w-7xl"
                src="../../assets/images/advertisement/hsc-adv.png"
                alt="HSC Advertisement"
              />
            </div>
            <div class="h-40 carousel-item">
              <img
                class="flex items-center w-40 h-24 mx-auto mt-4 d-block max-w-7xl"
                src="../../assets/images/advertisement/toyoda-adv.png"
                alt="Toyoda Goseio Advertisement"
              />
            </div>
          </div>

          <a
            class="carousel-control-prev"
            href="#carouselExampleControls"
            role="button"
            data-slide="prev"
          >
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a
            class="carousel-control-next"
            href="#carouselExampleControls"
            role="button"
            data-slide="next"
          >
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>

      <div class="absolute inset-0 px-6 top-24">
        <h3
          class="block text-xl font-normal text-left text-gray-900 sm:block md:hidden xl:hidden"
          data-aos-duration="1000"
          data-aos-once="true"
          data-aos="zoom-in-right"
        >
          TRUSTED BY
        </h3>
      </div>
    </div>
  </div>
</template>

<script setup>
import { defineComponent, ref } from 'vue'
</script>

<style scoped>
.align-center {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px 0 300px;
}

.web-advertisement {
  display: block;
}

@media only screen and (max-width: 766px) {
  .web-advertisement {
    display: none;
  }
}
</style>
