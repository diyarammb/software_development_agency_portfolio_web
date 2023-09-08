<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <login-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import LoginArea from '~~/components/login-register/LoginArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderOne,
    LoginArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Login - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
