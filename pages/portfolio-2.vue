
<template>
  <div>
    <header-one :top_bar="false" :transparent="true" :commonOffcanvas="true" />
    <portfolio-breadcrumb/>
    <grid-three-columns/>
    <start-up-cta :style_2="true"/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import PortfolioBreadcrumb from '~~/components/breadcrumb/PortfolioBreadcrumb.vue';
import StartUpCta from '~~/components/cta/StartUpCta.vue';
import GridThreeColumns from '~~/components/portfolios/portfolio-page/GridThreeColumns.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: { HeaderOne, PortfolioBreadcrumb, GridThreeColumns, StartUpCta, FooterSix, BackToTop},
  setup() {
    useHead({
      title: "Portfolio 2 - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
