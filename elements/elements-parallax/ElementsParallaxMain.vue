<template>
  <common-breadcrumb
    title="Have a look to our parallax background"
    subtitle="Elements"
  />
  <full-width-parallax-el/>
  <container-parallax-el/>
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import ContainerParallaxEl from './ContainerParallaxEl.vue';
import FullWidthParallaxEl from './FullWidthParallaxEl.vue';

export default {
  components: { CommonBreadcrumb, FullWidthParallaxEl, ContainerParallaxEl },
};
</script>

