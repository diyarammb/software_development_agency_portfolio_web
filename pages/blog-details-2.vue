<template>
  <div>
    <header-one :header_solid="true" :commonOffcanvas="true" />
    <blog-details-area-two />
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import BlogDetailsAreaTwo from "~~/components/blog-details/BlogDetailsAreaTwo.vue";
import Footer from "~~/layouts/footers/Footer.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: { HeaderOne, Footer, BackToTop, BlogDetailsAreaTwo },
  setup() {
    useHead({
      title: "Blog Details - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
