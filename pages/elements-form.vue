<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <element-form-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementFormMain from '~~/elements/elements-form/ElementFormMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementFormMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Form - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
