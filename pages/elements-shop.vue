<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-shop-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElShopMain from '~~/elements/elements-shop/ElShopMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElShopMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Shop - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
