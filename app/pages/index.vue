<template>
  <div>
    <HeroSection />
    <FeaturedSlider />

    <ServiceSection />
    <CustomerFeedback />
    <NewsSection />
  </div>
</template>

<script setup>
import HeroSection from "../components/home/HeroSection.vue";
import FeaturedSlider from "../components/home/FeaturedSlider.vue";
import ServiceSection from "../components/home/ServiceSection.vue";
import CustomerFeedback from "../components/home/CustomerFeedback.vue";
import NewsSection from "../components/home/NewsSection.vue";
</script>
