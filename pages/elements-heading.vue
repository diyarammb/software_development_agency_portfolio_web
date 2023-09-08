<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-heading-main />
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsHeadingMain from '~~/elements/elements-heading/ElementsHeadingMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsHeadingMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Heading - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
