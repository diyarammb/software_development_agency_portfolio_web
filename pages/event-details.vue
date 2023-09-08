<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <event-details-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import EventDetailsArea from '~~/components/event-details/EventDetailsArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    EventDetailsArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Event Details - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
