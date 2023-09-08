<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-brands-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsBrandsMain from '~~/elements/elements-brands/ElementsBrandsMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,

    Footer,
    BackToTop,
    ElementsBrandsMain,
  },
  setup() {
    useHead({
      title: "Element brands - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
