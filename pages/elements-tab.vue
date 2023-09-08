<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-tabs-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElTabsMain from '~~/elements/elements-tab/ElTabsMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElTabsMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Tab - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
