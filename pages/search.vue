<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <search-area/>
    <search-items/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import SearchArea from '~~/components/search/SearchArea.vue';
import SearchItems from '~~/components/search/SearchItems.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    SearchArea,
    SearchItems,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Search - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
