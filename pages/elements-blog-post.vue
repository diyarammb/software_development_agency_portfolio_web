<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-blog-post-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsBlogPostMain from '~~/elements/elements-blog-post/ElementsBlogPostMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementsBlogPostMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Blog Post - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
