<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-subscribe-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElSubscribeMain from '~~/elements/elements-subscribe/ElSubscribeMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElSubscribeMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Subscribe - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
