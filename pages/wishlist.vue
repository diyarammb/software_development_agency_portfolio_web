<template>
  <div>
    <header-twelve :style_2="true" />
    <cart-breadcrumb title="My Wishlist" subtitle="Wishlist" />
    <wishlist-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderTwelve from '~~/layouts/headers/HeaderTwelve.vue';
import CartBreadcrumb from '~~/components/breadcrumb/CartBreadcrumb.vue';
import WishlistArea from '~~/components/cart-wishlist/WishlistArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderTwelve,
    CartBreadcrumb,
    WishlistArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Wishlist - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
