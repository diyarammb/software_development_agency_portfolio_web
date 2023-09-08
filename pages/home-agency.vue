<template>
  <layout>
    <agency-hero/>
    <agency-services/>
    <agency-about/>
    <agency-counter/>
    <agency-portfolio/>
    <agency-awards/>
    <agency-pricing/>
    <agency-testimonial/>
    <agency-brands/>
    <agency-blogs/>
    <agency-cta/>
  </layout>
</template>

<script setup>
import layout from '~/layouts/LayoutFour.vue';
import AgencyHero from '~/components/hero-banner/AgencyHero.vue';
import AgencyServices from '~/components/services/AgencyServices.vue';
import AgencyAbout from '~/components/abouts/AgencyAbout.vue';
import AgencyCounter from '~/components/counters/AgencyCounter.vue';
import AgencyPortfolio from '~/components/portfolios/AgencyPortfolio.vue';
import AgencyAwards from '~/components/awards/AgencyAwards.vue';
import AgencyPricing from '~/components/pricing/AgencyPricing.vue';
import AgencyTestimonial from '~/components/testimonials/AgencyTestimonial.vue';
import AgencyBrands from '~/components/brands/AgencyBrands.vue';
import AgencyBlogs from '~/components/blogs/AgencyBlogs.vue';
import AgencyCta from '~~/components/cta/AgencyCta.vue';


useHead({
  title: "Home Agency - Creative Agency & Portfolio Vue Nuxt 3 Template",
}); 

</script>
