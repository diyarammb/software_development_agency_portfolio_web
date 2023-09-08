<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-gallery-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsGalleryMain from '~~/elements/elements-gallery/ElementsGalleryMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementsGalleryMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Gallery - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
