<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-parallax-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsParallaxMain from '~~/elements/elements-parallax/ElementsParallaxMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsParallaxMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Parallax - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
