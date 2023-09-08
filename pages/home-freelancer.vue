<template>
  <layout>
    <freelancer-hero/>
    <freelancer-brands/>
    <freelancer-about/>
    <freelancer-portfolio/>
    <freelancer-skills/>
    <freelancer-awards/>
    <freelancer-testimonial/>
    <freelancer-blogs/>
    <freelancer-cta/>
  </layout>
</template>

<script setup>
import layout from '~/layouts/LayoutThree.vue';
import FreelancerHero from '~/components/hero-banner/FreelancerHero.vue';
import FreelancerBrands from '~/components/brands/FreelancerBrands.vue';
import FreelancerAbout from '~/components/abouts/FreelancerAbout.vue';
import FreelancerPortfolio from '~/components/portfolios/FreelancerPortfolio.vue';
import FreelancerSkills from '~/components/skills/FreelancerSkills.vue';
import FreelancerAwards from '~/components/awards/FreelancerAwards.vue';
import FreelancerTestimonial from '~/components/testimonials/FreelancerTestimonial.vue';
import FreelancerBlogs from '~/components/blogs/FreelancerBlogs.vue';
import FreelancerCta from '~/components/cta/FreelancerCta.vue';


useHead({
  title: "Home Freelancer - Creative Agency & Portfolio Vue Nuxt 3 Template",
}); 

</script>
