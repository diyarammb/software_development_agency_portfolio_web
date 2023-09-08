<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <element-icon-box-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementIconBoxMain from '~~/elements/elements-iconbox/ElementIconBoxMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementIconBoxMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element IconBox - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
