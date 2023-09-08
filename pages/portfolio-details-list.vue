<template>
  <div>
    <header-one :top_bar="false" :header_black="true" :commonOffcanvas="true" />
    <list-with-details/>
    <footer-five :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ListWithDetails from '~~/components/portfolio-details/list-with-details/ListWithDetails.vue';
import FooterFive from '~~/layouts/footers/FooterFive.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: { HeaderOne, ListWithDetails, FooterFive, BackToTop},
  setup() {
    useHead({
      title: "Portfolio Details List - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  }, 
};
</script>
