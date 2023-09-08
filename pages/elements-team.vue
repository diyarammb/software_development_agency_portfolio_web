<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-team-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsTeamMain from '~~/elements/elements-team/ElementsTeamMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElementsTeamMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Team - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
