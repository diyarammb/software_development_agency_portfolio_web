<template>
  <common-breadcrumb
    title="Have a look to our instagram style"
    subtitle="Elements"
  />
  <slider-instagram-el />
  <instagram-grid-el />
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import InstagramGridEl from "./InstagramGridEl.vue";
import SliderInstagramEl from "./SliderInstagramEl.vue";
export default {
  components: { CommonBreadcrumb, SliderInstagramEl, InstagramGridEl },
};
</script>
