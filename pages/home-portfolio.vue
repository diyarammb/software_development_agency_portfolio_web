<template>
  <Layout>
    <personal-portfolio-hero/>
    <personal-port-about/>
    <personal-port-feature/>
    <personal-port-services/>
    <personal-port-portfolio/>
    <personal-port-skills/>
    <personal-port-awards/>
    <personal-port-testimonial/>
    <personal-port-blogs/>
    <personal-port-contact/>
  </Layout>
</template>

<script setup>
import Layout from "~/layouts/LayoutEight.vue";
import PersonalPortfolioHero from "~/components/hero-banner/PersonalPortfolioHero.vue";
import PersonalPortAbout from '~/components/abouts/PersonalPortAbout.vue';
import PersonalPortFeature from "~/components/features/PersonalPortFeature.vue";
import PersonalPortServices from "~/components/services/PersonalPortServices.vue";
import PersonalPortPortfolio from "~/components/portfolios/PersonalPortPortfolio.vue";
import PersonalPortSkills from "~/components/skills/PersonalPortSkills.vue";
import PersonalPortAwards from "~/components/awards/PersonalPortAwards.vue";
import PersonalPortTestimonial from "~/components/testimonials/PersonalPortTestimonial.vue";
import PersonalPortBlogs from "~/components/blogs/PersonalPortBlogs.vue";
import PersonalPortContact from "~/components/contact/PersonalPortContact.vue";

useHead({
  title: "Home Portfolio - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
