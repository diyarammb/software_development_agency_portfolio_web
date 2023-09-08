<template>
  <layout>
    <architecture-banner/>
    <architecture-about/>
    <architecture-counter/>
    <architecture-portfolio/>
    <architecture-services/>
    <architecture-awards/>
    <architecture-video/>
    <architecture-testimonial/>
    <architecture-teams/>
    <architecture-blogs/>
  </layout>
</template>

<script setup>
import layout from "~/layouts/LayoutNine.vue";
import ArchitectureBanner from "~/components/hero-banner/ArchitectureBanner.vue";
import ArchitectureAbout from "~/components/abouts/ArchitectureAbout.vue";
import ArchitectureCounter from "~/components/counters/ArchitectureCounter.vue";
import ArchitecturePortfolio from "~/components/portfolios/ArchitecturePortfolio.vue";
import ArchitectureServices from "~/components/services/ArchitectureServices.vue";
import ArchitectureAwards from "~/components/awards/ArchitectureAwards.vue";
import ArchitectureVideo from "~/components/video-area/ArchitectureVideo.vue";
import ArchitectureTestimonial from "~/components/testimonials/ArchitectureTestimonial.vue";
import ArchitectureTeams from "~/components/teams/ArchitectureTeams.vue";
import ArchitectureBlogs from "~/components/blogs/ArchitectureBlogs.vue";

useHead({
  title: "Home Architecture - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
