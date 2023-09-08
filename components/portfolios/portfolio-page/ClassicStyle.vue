<template>
  <section class="portfolio__area pt-110 pb-75 p-relative fix">
    <div class="portfolio__shape">
      <img
        class="portfolio__shape-13"
        src="~/assets/img/portfolio/grid/shape/circle-1.png"
        alt=""
      />
      <img
        class="portfolio__shape-14"
        src="~/assets/img/portfolio/grid/shape/circle-2.png"
        alt=""
      />
      <img
        class="portfolio__shape-15"
        src="~/assets/img/portfolio/grid/shape/circle-sm.png"
        alt=""
      />
      <img
        class="portfolio__shape-16"
        src="~/assets/img/portfolio/grid/shape/polygon-yellow.png"
        alt=""
      />
      <img
        class="portfolio__shape-17"
        src="~/assets/img/portfolio/grid/shape/polygon-pink.png"
        alt=""
      />
      <img
        class="portfolio__shape-18"
        src="~/assets/img/portfolio/grid/shape/polygon-green.png"
        alt=""
      />
      <img
        class="portfolio__shape-19"
        src="~/assets/img/portfolio/grid/shape/polygon-green-2.png"
        alt=""
      />
    </div>
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div class="portfolio__section-title-wrapper text-center mb-90">
            <span class="portfolio__section-title-pre">
              CHECK OUT OUR LATEST WORK
            </span>
            <h3 class="portfolio__section-title">Portfolio Classic</h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-xxl-12">
          <div class="portfolio__masonary-btn text-center mb-40">
            <div class="masonary-menu filter-button-group">
              <button
                v-for="(cate, i) in categories"
                :key="i"
                @click="handleCategoryItem(cate)"
                :class="`${cate === activeCategory ? 'active' : ''}`"
              >
                {{ cate }}

                <span>
                  {{
                    cate === "All"
                      ? portfolio_data.length
                      : portfolio_data.filter((item) => item.category === cate)
                          .length
                  }}
                </span>
              </button>
            </div>
          </div>
        </div>
      </div>
      <transition-group
        name="list"
        tag="div"
        appear
        class="row tp-gx-4 grid tp-portfolio-load-more"
        ref="product_ref"
      >
        <div
          v-for="(item, i) in portfolio_items?.slice(0, perView)"
          :key="i"
          :data-index="i"
          class="col-xl-4 col-lg-4 col-md-6 tp-portfolio grid-item"
        >
          <classic-single-item
            :item="item"
            :index="i"
            :images="portfolio_items.map((item) => item.img)"
          />
        </div>
      </transition-group>
      <div class="row">
        <div class="col-xxl-12">
          <div class="portfolio__load-more text-center">
            <button
              v-if="perView < portfolio_items.length"
              @click="handleLoadMore()"
              id="tp-load-more"
              type="button"
              class="tp-load-more-btn load-more mt-30 mb-50"
            >
              <svg
                width="17"
                height="17"
                viewBox="0 0 17 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M1 8.5C1 4.36 4.33 1 8.5 1C13.5025 1 16 5.17 16 5.17M16 5.17V1.42M16 5.17H12.67"
                  stroke="currentColor"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M15.9175 8.5C15.9175 12.64 12.5575 16 8.4175 16C4.2775 16 1.75 11.83 1.75 11.83M1.75 11.83H5.14M1.75 11.83V15.58"
                  stroke="currentColor"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              Load more Post
            </button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import { ref, onMounted } from "vue";
// internal
import img_1 from "~/assets/img/portfolio/grid/portfolio-grid-1.jpg";
import img_2 from "~/assets/img/portfolio/grid/portfolio-grid-2.jpg";
import img_3 from "~/assets/img/portfolio/grid/portfolio-grid-3.jpg";
import img_4 from "~/assets/img/portfolio/grid/portfolio-grid-4.jpg";
import img_5 from "~/assets/img/portfolio/grid/portfolio-grid-5.jpg";
import img_6 from "~/assets/img/portfolio/grid/portfolio-grid-6.jpg";
import img_7 from "~/assets/img/portfolio/grid/portfolio-grid-7.jpg";
import img_8 from "~/assets/img/portfolio/grid/portfolio-grid-8.jpg";
import img_9 from "~/assets/img/portfolio/grid/portfolio-grid-9.jpg";
import img_10 from "~/assets/img/portfolio/grid/portfolio-grid-10.jpg";
import img_11 from "~/assets/img/portfolio/grid/portfolio-grid-11.jpg";
import img_12 from "~/assets/img/portfolio/grid/portfolio-grid-12.jpg";
import ClassicSingleItem from "./ClassicSingleItem.vue";

export default {
  components: { ClassicSingleItem },
  data() {
    return {
      perView: 6,
      categories: [],
      activeCategory: "All",
      portfolio_items: [],
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
          category: "Branding",
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
          category: "Apps",
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
        {
          id: "7",
          img: img_7,
          title: "Visual Identity",
          category: "Creative",
        },
        {
          id: "8",
          img: img_8,
          title: "UX Web Design",
          category: "Creative",
          video: true,
          video_id: "ty8Y0hCJIYw",
        },
        {
          id: "9",
          img: img_9,
          title: "Magazine Cover",
          category: "Creative",
        },
        {
          id: "10",
          img: img_10,
          title: "Visual Identity",
          category: "Packaging",
        },
        {
          id: "11",
          img: img_11,
          title: "UX Web Design",
          category: "Packaging",
          video: true,
          video_id: "Xm2VKy2a6aQ",
        },
        {
          id: "12",
          img: img_12,
          title: "Magazine Cover",
          category: "Mockup",
        },
      ],
    };
  },
  methods: {
    handleCategoryItem(value) {
      this.activeCategory = value;
      this.perView = this.perView;
      if (value === "All") {
        this.portfolio_items = this.portfolio_data;
      } else {
        this.portfolio_items = this.portfolio_data.filter(
          (item) => item.category === value
        );
      }
    },
    // handleLoadMore
    handleLoadMore() {
      this.perView = this.perView + 3;
    },
  },
  created() {
    this.categories = [
      "All",
      ...new Set(this.portfolio_data.map((item) => item.category)),
    ];
    this.portfolio_items = this.portfolio_data;
  },
};
</script>

<style>
.list-enter-active,
.list-leave-active {
  transition: all 0.5s ease;
}
.list-enter-from{
  opacity: 0;
  transform: translateY(-30px);
}
.list-enter-to{
  opacity: 1;
  transform: translateY(0px);
}
.list-leave-from{
  opacity: 1;
  transform: translateY(0px);
}
.list-leave-to {
  opacity: 0;
  transform: translateX(-30px);
}
</style>
