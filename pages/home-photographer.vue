<template>
  <layout>
    <photographer-hero />
    <photographer-about />
    <photographer-portfolio />
    <photography-pricing />
    <photographer-services />
    <photographer-review />
    <photographer-testimonial />
    <photographer-brands/>
    <photographer-instagram/>
  </layout>
</template>

<script setup>
import layout from "~/layouts/LayoutFive.vue";
import PhotographerHero from "~/components/hero-banner/PhotographerHero.vue";
import PhotographerAbout from "~/components/abouts/PhotographerAbout";
import PhotographerPortfolio from "~/components/portfolios/PhotographerPortfolio.vue";
import PhotographyPricing from "~/components/pricing/PhotographyPricing.vue";
import PhotographerServices from "~/components/services/PhotographerServices.vue";
import PhotographerReview from "~/components/review-area/PhotographerReview.vue";
import PhotographerTestimonial from "~/components/testimonials/PhotographerTestimonial.vue";
import PhotographerBrands from '~/components/brands/PhotographerBrands.vue';
import PhotographerInstagram from '~/components/instagram/PhotographerInstagram.vue';

useHead({
  title: "Home Photographer - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
