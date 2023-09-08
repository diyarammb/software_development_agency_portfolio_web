<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <start-up-pricing :style_2="true" />
    <pricing-testimonial/>
    <common-faq padd="120"/>
    <about-cta/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import StartUpPricing from "~~/components/pricing/StartUpPricing";
import PricingTestimonial from '~~/components/testimonials/PricingTestimonial.vue';
import CommonFaq from '~~/components/faqs/CommonFaq.vue';
import AboutCta from '~~/components/cta/AboutCta.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    StartUpPricing,
    PricingTestimonial,
    FooterSix,
    AboutCta,
    BackToTop,
    CommonFaq,
  },
  setup() {
    useHead({
      title: "Pricing - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
