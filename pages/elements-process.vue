<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-process-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsProcessMain from '~~/elements/elements-process/ElementsProcessMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsProcessMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Process - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
