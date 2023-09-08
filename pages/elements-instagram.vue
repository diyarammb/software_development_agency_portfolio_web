<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-instagram-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsInstagramMain from '~~/elements/elements-instagram/ElementsInstagramMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsInstagramMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element instagram - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
