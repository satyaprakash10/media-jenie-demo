<template>
  <footer class="px-4 pt-20 bg-black xl:px-0">
    <div
      class="grid grid-cols-1 gap-10 px-4 mx-auto max-w-7xl md:grid-cols-3 sm:grid-cols-2"
    >
      <div>
        <div
          data-aos="fade-down"
          data-aos-easing="linear"
          data-aos-duration="1000"
        >
          <img
            class="cursor-pointer"
            src="../../assets/images/mediajenie-white-logo.png"
            width="146"
            height="55"
          />
        </div>

        <div class="flex items-center justify-start mt-4 space-x-3">
          <a
            data-aos="fade-up"
            data-aos-duration="100"
            href="#"
            class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-90 hover:shadow-2xl"
          >
            <img
              src="../../assets/images/social-icons/instagram.png"
              alt=""
              height="50"
              width="50"
            />
          </a>
          <a
            data-aos="fade-up"
            data-aos-duration="500"
            href="#"
            class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-90 hover:shadow-2xl"
          >
            <img
              src="../../assets/images/social-icons/twitter.png"
              alt=""
              height="50"
              width="50"
            />
          </a>
          <a
            href="#"
            class="transition-all duration-500 ease-in-out transform cursor-pointer hover:scale-90 hover:shadow-2xl"
          >
            <img
              src="../../assets/images/social-icons/linkedin.png"
              alt=""
              height="50"
              width="50"
            />
          </a>
        </div>
      </div>

      <div class="col-span-2">
        <h4
          class="text-3xl font-semibold text-white"
          data-aos="zoom-out-right"
          data-aos-duration="1000"
        >
          About the company
        </h4>

        <p
          data-aos="zoom-out-left"
          data-aos-duration="1000"
          class="my-4 text-base font-normal text-white"
        >
          MediaJenie is a digital transformation agency. We bring your brand &
          customers closer through strategy, creativity, content & digital
          solutions powered by data analytics. From start-ups to SMEs and large
          corporations, we have successfully designed and delivered different
          media solutions.
        </p>

        <div data-aos="zoom-out-up" data-aos-duration="1000">
          <button
            class="z-40 px-6 py-2.5 text-xl font-normal text-black transition-all duration-500 ease-in btn hover:bg-yellow-600 hover:shadow-xl"
          >
            Read More
          </button>
        </div>
      </div>
    </div>

    <div class="w-full mt-10 border-b border-gray-600"></div>

    <p
      class="py-5 text-sm font-normal text-center text-gray-400 cursor-pointer hover:text-yellow-400"
    >
      MediaJenie, Bangalore, India
    </p>
  </footer>
</template>

<script setup>
import SiteLogo from '../../components/icons/SiteLogo.vue'
</script>

<style scoped>
.btn {
  background: #fdcc06;
  color: #000000;
  cursor: pointer;
  border-radius: 0px;
  position: relative;
  overflow: hidden;
  transition: all 0.5s;
}

.btn:before {
  width: 144px;
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
</style>
