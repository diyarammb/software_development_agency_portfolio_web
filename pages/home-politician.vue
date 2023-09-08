<template>
  <layout>
    <home-politician-banner/>
    <politician-cta/>
    <politician-feature/>
    <politician-vision/>
    <politician-counter/>
    <politician-events/>
    <polity-biography-area/>
    <polity-teams/>
    <polity-donate-area/>
    <politician-blogs/>
    <politician-testimonial/>
    <politician-subscribe/>
  </layout>
</template>

<script setup>
import layout from "~/layouts/LayoutEleven.vue";
import HomePoliticianBanner from "~/components/hero-banner/HomePoliticianBanner.vue";
import PoliticianCta from "~/components/cta/PoliticianCta.vue";
import PoliticianFeature from "~/components/features/PoliticianFeature.vue";
import PoliticianVision from "~/components/vision/PoliticianVision.vue";
import PoliticianCounter from "~/components/counters/PoliticianCounter.vue";
import PoliticianEvents from "~/components/events/PoliticianEvents.vue";
import PolityBiographyArea from "~/components/biography/PolityBiographyArea.vue";
import PolityTeams from "~/components/teams/PolityTeams.vue";
import PolityDonateArea from "~/components/donate-area/PolityDonateArea.vue";
import PoliticianBlogs from "~/components/blogs/PoliticianBlogs.vue";
import PoliticianTestimonial from "~/components/testimonials/PoliticianTestimonial.vue";
import PoliticianSubscribe from "~/components/subscribe/PoliticianSubscribe.vue";

useHead({
  title: "Home Politician - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
