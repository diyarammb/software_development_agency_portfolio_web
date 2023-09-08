<template>
  <div>
    <header-one :top_bar="false" :header_black="true" :commonOffcanvas="true" />
    <details-with-video/>
    <footer-five :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import FooterFive from '~~/layouts/footers/FooterFive.vue';
import DetailsWithVideo from '~~/components/portfolio-details/details-with-video/DetailsWithVideo.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: { HeaderOne, FooterFive, DetailsWithVideo, BackToTop},
  setup() {
    useHead({
      title: "Portfolio Details Video - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  }, 
};
</script>
