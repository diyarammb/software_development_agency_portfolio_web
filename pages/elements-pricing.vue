<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-pricing-main />
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsPricingMain from "~~/elements/elements-pricing/ElementsPricingMain.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsPricingMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Pricing - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
