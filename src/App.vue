<template>
  <div class="overflow-x-hidden bg-gray-50 body">
    <!-- The site Navbar -->
    <HeaderSection />

    <!-- Site advertisement container -->
    <AdvertisementSection />

    <!-- Site get quote  -->
    <SiteQuote />

    <!-- Site Capability & Feature container  -->
    <CapabilitySection />

    <!-- Site work section  -->
    <WorkSection />

    <!-- Site view more adv work section  -->
    <ViewMoreWork />

    <!-- Site Basic Footer section  -->
    <FooterSection />

    <div class="body-footer"></div>
  </div>
</template>

<script setup>
import HeaderSection from './components/HeaderSection.vue'
import AdvertisementSection from '../src/assets/views/AdvertisementSection.vue'
import SiteQuote from '../src/assets/views/SiteQuote.vue'
import CapabilitySection from '../src/assets/views/CapabilitySection.vue'
import WorkSection from '../src/assets/views/WorkSection.vue'
import ViewMoreWork from '../src/assets/views/ViewMoreWork.vue'
import FooterSection from '../src/assets/views/FooterSection.vue'
</script>

<style scoped lang="css"></style>
