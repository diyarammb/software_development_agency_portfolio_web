<template>
  <div>
    <header-twelve :style_2="true" />
    <cart-breadcrumb title="Checkout" subtitle="Checkout" />
    <coupon-area/>
    <checkout-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderTwelve from '~~/layouts/headers/HeaderTwelve.vue';
import CartBreadcrumb from '~~/components/breadcrumb/CartBreadcrumb.vue';
import CouponArea from '~~/components/checkout/CouponArea.vue';
import CheckoutArea from '~~/components/checkout/CheckoutArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderTwelve,
    CartBreadcrumb,
    CouponArea,
    CheckoutArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Checkout - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
