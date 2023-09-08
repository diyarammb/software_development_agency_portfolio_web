<template>
  <common-breadcrumb
    title="Have a look to our shop styles"
    subtitle="Elements"
  />
  <shop-category :el_style="true" />
  <el-shop-category-grid />
  <div class="tp-separator"></div>
  <el-shop-product-grid />
  <el-shop-product-list/>
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import ShopCategory from "~~/components/shop/ShopCategory.vue";
import ElShopCategoryGrid from "./ElShopCategoryGrid.vue";
import ElShopProductGrid from "./ElShopProductGrid.vue";
import ElShopProductList from './ElShopProductList.vue';

export default {
  components: {
    CommonBreadcrumb,
    ShopCategory,
    ElShopCategoryGrid,
    ElShopProductGrid,
    ElShopProductList,
  },
};
</script>
