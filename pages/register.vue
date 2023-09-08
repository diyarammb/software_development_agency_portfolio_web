<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <register-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import RegisterArea from '~~/components/login-register/RegisterArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderOne,
    RegisterArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Register - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
