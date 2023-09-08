<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <element-button-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementButtonMain from '~~/elements/elements-button/ElementButtonMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementButtonMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element button - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
