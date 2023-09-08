<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-video-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElVideoMain from '~~/elements/elements-video/ElVideoMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElVideoMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Video - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
