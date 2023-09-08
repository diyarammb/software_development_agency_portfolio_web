<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <metro-style/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import Footer from '~~/layouts/footers/Footer.vue';
import MetroStyle from '~~/components/portfolios/portfolio-page/MetroStyle.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: { HeaderOne, Footer, MetroStyle, BackToTop},
  setup() {
    useHead({
      title: "Portfolio Metro - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
