<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <details-slider/>
    <footer-five :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import DetailsSlider from '~~/components/portfolio-details/details-slider/DetailsSlider.vue';
import FooterFive from '~~/layouts/footers/FooterFive.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: { HeaderOne, DetailsSlider, FooterFive, BackToTop},
  setup() {
    useHead({
      title: "Portfolio Details Slider - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  }, 
};
</script>
