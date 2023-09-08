<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
     <services-breadcrumb-two/>
    <services-area-two/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ServicesBreadcrumbTwo from '~~/components/breadcrumb/ServicesBreadcrumbTwo.vue';
import ServicesAreaTwo from '~~/components/services/ServicesAreaTwo.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    ServicesBreadcrumbTwo,
    ServicesAreaTwo,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Services 2 - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
