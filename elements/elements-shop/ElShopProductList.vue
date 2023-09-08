<template>
  <section class="product__popular-area pt-110 pb-90">
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
            <h3 class="tp-section-title-3">Shop Product List</h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div
          v-for="(item, i) in productData.slice(0, 5)"
          :key="i"
          class="col-lg-12 col-md-6"
        >
          <single-list-product :item="item" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SingleListProduct from "~~/components/shop/SingleListProduct.vue";
import productData from "~~/mixins/productData";

export default {
  components: { SingleListProduct },
  mixins: [productData],
};
</script>
