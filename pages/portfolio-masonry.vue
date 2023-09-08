<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <portfolio-masonry/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import PortfolioMasonry from '~~/components/portfolios/portfolio-page/PortfolioMasonry.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";

export default {
  components: { HeaderOne, PortfolioMasonry, Footer, BackToTop},
  setup() {
    useHead({
      title: "Portfolio Masonry - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
