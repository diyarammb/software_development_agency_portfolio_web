<template>
  <section class="portfolio__area pt-110 pb-70">
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div class="section__title-wrapper-9 text-center mb-55">
            <h3 class="section__title">Latest Projects</h3>
          </div>
        </div>
      </div>
      <div class="row tp-gx-4">
        <div
          v-for="(item, i) in portfolio_data"
          :key="i"
          class="col-xl-4 col-lg-4 col-md-6"
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
import img_4 from "~/assets/img/portfolio/grid/portfolio-grid-4.jpg";
import img_5 from "~/assets/img/portfolio/grid/portfolio-grid-5.jpg";
import img_6 from "~/assets/img/portfolio/grid/portfolio-grid-6.jpg";
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
        {
          id: "4",
          img: img_4,
          title: "Product Design",
          category: "Branding",
        },
        {
          id: "5",
          img: img_5,
          title: "Branding Design",
          category: "Branding",
        },
        {
          id: "6",
          img: img_6,
          title: "Original Coffee",
          category: "Creative",
          video: true,
          video_id: "1gyTUHP6ne8",
        },
      ],
    };
  },
};
</script>
