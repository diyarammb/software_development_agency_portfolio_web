<template>
  <div>
    <header-twelve :style_2="true" />
    <cart-breadcrumb title="My Cart" subtitle="Cart" />
    <cart-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderTwelve from '~~/layouts/headers/HeaderTwelve.vue';
import CartBreadcrumb from '~~/components/breadcrumb/CartBreadcrumb.vue';
import CartArea from '~~/components/cart-wishlist/CartArea.vue';

import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderTwelve,
    CartArea,
    CartBreadcrumb,

    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Cart - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
