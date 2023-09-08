<template>
  <div>
    <header-thirteen />
    <swipper-slider/>
  </div>
</template>

<script>
import HeaderThirteen from "~~/layouts/headers/HeaderThirteen.vue";
import SwipperSlider from "~/components/swipper-slider/SwipperSlider.vue";

export default {
  components: { HeaderThirteen,SwipperSlider },
  setup() {
    useHead({
      title: "Home Swiper - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
