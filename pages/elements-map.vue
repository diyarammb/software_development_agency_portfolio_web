<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-map-main />
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsMapMain from "~~/elements/elements-map/ElementsMapMain.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsMapMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Map - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
