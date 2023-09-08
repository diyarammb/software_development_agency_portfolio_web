<template>
 <section class="product__category pt-10 pb-100">
  <div class="container">
      <div class="row">
        <div class="col-xxl-12">
            <div class="tp-section-wrapper-3 mb-60 text-center">
              <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
              <h3 class="tp-section-title-3">Shop Category Grid</h3>
            </div>
        </div>
      </div>
      <div class="row">
        <div v-for="(item, i) in products_category" :key="i" class="col-xl-3 col-lg-3 col-md-6 col-sm-6">
            <div class="product__category-item mb-20 text-center swiper-slide">
              <div class="product__category-thumb w-img">
                  <nuxt-link href="/shop">
                    <img :src="item.img" alt="">
                  </nuxt-link>
              </div>
              <div class="product__category-content">
                  <h3 class="product__category-title">
                    <nuxt-link href="/shop">{{item.title}}</nuxt-link>
                  </h3>
              </div>
            </div>
        </div>
      </div>
  </div>
</section>
</template>

<script>
// internal
import cate_1 from "~/assets/img/product/category/product-cat-1.jpg";
import cate_2 from "~/assets/img/product/category/product-cat-2.jpg";
import cate_3 from "~/assets/img/product/category/product-cat-3.jpg";
import cate_4 from "~/assets/img/product/category/product-cat-4.jpg";

  export default {
    data() {
    return {
      products_category: [
        {
          img: cate_1,
          title: "Call Phone &Tablets",
        },
        {
          img: cate_2,
          title: "Game & Video",
        },
        {
          img: cate_3,
          title: "Sport Watches",
        },
        {
          img: cate_4,
          title: "Computers & Laptop",
        },
      ],
    };
  },
  }
</script>
