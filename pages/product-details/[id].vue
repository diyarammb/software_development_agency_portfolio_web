<template>
  <div>
    <header-twelve :style_2="true" />
    <product-details-breadcrumb />
    <product-details-area :item="item" />
    <product-details-tab-area />
    <related-products />
    <shop-cta />
    <footer-eleven />
    <back-to-top />
  </div>
</template>

<script>
import productData from "~~/mixins/productData";
import HeaderTwelve from "~~/layouts/headers/HeaderTwelve.vue";
import ProductDetailsBreadcrumb from "~~/components/breadcrumb/ProductDetailsBreadcrumb.vue";
import ProductDetailsArea from "~~/components/product-details/ProductDetailsArea.vue";
import ShopCta from "~~/components/cta/ShopCta.vue";
import ProductDetailsTabArea from "~~/components/product-details/ProductDetailsTabArea.vue";
import RelatedProducts from "~~/components/product-details/RelatedProducts.vue";
import FooterEleven from "~~/layouts/footers/FooterEleven.vue";
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";

export default {
  components: {
    HeaderTwelve,
    ProductDetailsBreadcrumb,
    ShopCta,
    ProductDetailsArea,
    ProductDetailsTabArea,
    RelatedProducts,
    FooterEleven,
    BackToTop,
  },
  mixins: [productData],
  data() {
    return {
      item: {},
    };
  },
  setup() {
    useHead({
      title:
        "Product Details - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
  created() {
    const route = useRoute();
    this.item = productData
      .data()
      .productData.find((p) => p.id == route.params.id);
  },
};
</script>
