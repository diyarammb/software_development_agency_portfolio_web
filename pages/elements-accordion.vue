<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <elements-accordion-main/>
    <Footer/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElementsAccordionMain from '~/elements/elements-accordion/ElementsAccordionMain.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';
import Footer from '~~/layouts/footers/Footer.vue';

export default {
  components: {
    HeaderOne,
    ElementsAccordionMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Element Accordion - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
