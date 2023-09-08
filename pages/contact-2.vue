<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <contact-area-two/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ContactAreaTwo from '~~/components/contact/ContactAreaTwo.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    ContactAreaTwo,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Contact 2 - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
