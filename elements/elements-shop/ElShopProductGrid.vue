<template>
  <section class="product__popular-area pt-110 pb-20">
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
            <h3 class="tp-section-title-3">Shop Product Grid</h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div
          v-for="(item, i) in productData.slice(0, 8)"
          :key="i"
          class="col-xl-3 col-lg-4 col-md-6 col-sm-6"
        >
          <single-product :item="item" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SingleProduct from "~~/components/shop/SingleProduct.vue";
import productData from "~~/mixins/productData";

export default {
  components: { SingleProduct },
  mixins: [productData],
};
</script>
