<template>
  <section class="portfolio__area pt-110 pb-75 p-relative fix">
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
            <h3 class="tp-section-title-3">Gallery Grid Style</h3>
          </div>
        </div>
      </div>
      <div class="row tp-gx-4">
        <div
          v-for="(item, i) in portfolio_data"
          :key="i"
          class="col-xl-4 col-lg-4 col-md-6 tp-portfolio grid-item"
        >
          <classic-single-item
            :item="item"
            :index="i"
            :images="portfolio_data.map((item) => item.img)"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import img_1 from "~/assets/img/portfolio/grid/portfolio-grid-1.jpg";
import img_2 from "~/assets/img/portfolio/grid/portfolio-grid-2.jpg";
import img_3 from "~/assets/img/portfolio/grid/portfolio-grid-3.jpg";
import ClassicSingleItem from "~~/components/portfolios/portfolio-page/ClassicSingleItem.vue";

export default {
  components: { ClassicSingleItem },
  data() {
    return {
      portfolio_data: [
        {
          id: "1",
          img: img_1,
          title: "Magazine Cover",
          category: "Apps",
        },
        {
          id: "2",
          img: img_2,
          title: "Logo Mockups",
          category: "Apps",
        },
        {
          id: "3",
          img: img_3,
          title: "Pattern Inspired",
          category: "Apps",
        },
      ],
    };
  },
};
</script>
