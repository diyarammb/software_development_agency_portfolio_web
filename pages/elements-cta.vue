<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-cta-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsCtaMain from '~~/elements/elements-cta/ElementsCtaMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementsCtaMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Cta - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
