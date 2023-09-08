<template>
  <Layout>
    <start-up-banner/>
    <startup-features/>
    <start-up-about/>
    <start-up-counter/>
    <start-up-services/>
    <start-up-feature-list/>
    <start-up-support/>
    <start-up-testimonial/>
    <start-up-pricing/>
    <start-up-faq/>
    <start-up-blogs/>
    <start-up-cta/>
  </Layout>
</template>

<script setup>
import Layout from "~/layouts/LayoutSix.vue";
import StartUpBanner from "~/components/hero-banner/StartUpBanner.vue";
import StartupFeatures from "~/components/features/StartupFeatures.vue";
import StartUpAbout from '~/components/abouts/StartUpAbout.vue';
import StartUpCounter from "~/components/counters/StartUpCounter.vue";
import StartUpServices from "~/components/services/StartUpServices.vue";
import StartUpFeatureList from "~/components/features/StartUpFeatureList";
import StartUpSupport from '~/components/supports/StartUpSupport.vue';
import StartUpTestimonial from "~/components/testimonials/StartUpTestimonial.vue";
import StartUpPricing from '~/components/pricing/StartUpPricing';
import StartUpFaq from '~/components/faqs/StartUpFaq';
import StartUpBlogs from "~/components/blogs/StartUpBlogs.vue";
import StartUpCta from '~/components/cta/StartUpCta.vue';

useHead({
  title: "Home Startup - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
