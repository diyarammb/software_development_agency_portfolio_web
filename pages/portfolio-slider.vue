<template>
  <div>
    <header-one
      :top_bar="false"
      :header_solid="true"
      :header_solid_2="true"
      :commonOffcanvas="true"
    />
    <slider-portfolio />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import SliderPortfolio from "~~/components/portfolios/portfolio-page/SliderPortfolio.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: { HeaderOne, SliderPortfolio, BackToTop },
  setup() {
    useHead({
      title:
        "Portfolio Masonry - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
