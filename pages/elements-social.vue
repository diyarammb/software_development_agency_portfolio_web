<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-social-style-main />
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";

import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";
import ElSocialStyleMain from "~~/elements/elements-social/ElSocialStyleMain.vue";

export default {
  components: {
    HeaderOne,
    ElSocialStyleMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Social - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
