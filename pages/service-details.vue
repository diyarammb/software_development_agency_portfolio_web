<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <service-details-breadcrumb/>
    <service-details-area/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ServiceDetailsBreadcrumb from '~~/components/breadcrumb/ServiceDetailsBreadcrumb.vue';
import ServiceDetailsArea from '~~/components/service-details/ServiceDetailsArea.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    ServiceDetailsBreadcrumb,
    ServiceDetailsArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Services Details - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
