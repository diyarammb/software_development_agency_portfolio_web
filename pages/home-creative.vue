<template>
  <layout>
    <creative-hero/>
    <creative-feature/>
    <creative-about/>
    <creative-cta/>
    <creative-portfolio/>
    <creative-team/>
    <creative-blogs/>
    <creative-testimonial/>
    <creative-brands/>
    <creative-cta-two/>
  </layout>
</template>

<script setup>
import layout from "~/layouts/LayoutSeven.vue";
import CreativeHero from "~/components/hero-banner/CreativeHero.vue";
import CreativeFeature from "~/components/features/CreativeFeature.vue";
import CreativeAbout from '~/components/abouts/CreativeAbout.vue';
import CreativeCta from "~/components/cta/CreativeCta.vue";
import CreativePortfolio from "~/components/portfolios/CreativePortfolio.vue";
import CreativeTeam from "~/components/teams/CreativeTeam.vue";
import CreativeBlogs from "~/components/blogs/CreativeBlogs.vue";
import CreativeTestimonial from "~/components/testimonials/CreativeTestimonial.vue";
import CreativeBrands from '~/components/brands/CreativeBrands.vue';
import CreativeCtaTwo from "~/components/cta/CreativeCtaTwo.vue";

useHead({
  title: "Home Creative - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
