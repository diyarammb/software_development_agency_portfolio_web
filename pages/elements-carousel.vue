<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-carousel-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsCarouselMain from '~~/elements/elements-carousel-main/ElementsCarouselMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsCarouselMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Carousel - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
