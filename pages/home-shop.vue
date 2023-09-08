<template>
  <layout>
    <shop-hero-banner/>
    <shop-category/>
    <popular-product/>
    <shop-banner/>
    <shop-features/>
    <shop-cta/>
  </layout>
</template>

<script setup>
import layout from "~/layouts/LayoutTwelve.vue";
import ShopHeroBanner from '~/components/hero-banner/ShopHeroBanner.vue';
import ShopCategory from "~/components/shop/ShopCategory.vue";
import PopularProduct from "~/components/shop/PopularProduct.vue";
import ShopBanner from "~/components/shop/ShopBanner.vue";
import ShopFeatures from "~/components/shop/ShopFeatures.vue";
import ShopCta from "~/components/cta/ShopCta.vue";

useHead({
  title: "Home Shop - Creative Agency & Portfolio Vue Nuxt 3 Template",
});
</script>
