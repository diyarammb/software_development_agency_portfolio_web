<template>
  <section :class="`about__gallery-area fix ${el_style ? 'pt-120 pb-110' : ''}`">
    <div class="container">
      <div v-if="el_style" class="row">
        <div class="col-xxl-12">
            <div class="tp-section-wrapper-3 mb-60 text-center">
              <span class="tp-section-subtitle-3">Modern &amp; Clean Design</span>
              <h3 class="tp-section-title-3">Carousel With Arrow</h3>
            </div>
        </div>
      </div>
      <div class="row justify-content-center">
        <div class="col-xl-10 col-lg-10">
          <div class="about__gallery-slider pl-50 pr-50 p-relative">

            <Carousel ref="detailsSlider"
              :items-to-show="1"
              :wrap-around="true"
              :snapAlign="'center'"
              :breakpoints="{
                992: {
                  itemsToShow: 1,
                },
                700: {
                  itemsToShow: 1,
                },
                0: {
                  itemsToShow: 1,
                },
              }" 
              class="about__gallery-slider-active">
              <Slide v-for="(img, i) in images"
                :key="i" class="about__gallery-item">
                <div class="about__gallery-thumb m-img">
                  <img :src="img" alt="">
                </div>
              </Slide>
            </Carousel>

            <div class="about__gallery-arrow d-none d-sm-block">
              <button
                @click="handlePrev"
                type="button"
                class="about-button-prev slick-prev slick-arrow"
              >
                <span><i class="fa-regular fa-arrow-left"></i></span>
              </button>
              <button
                @click="handleNext"
                type="button"
                class="about-button-next slick-next slick-arrow"
              >
                <span><i class="fa-regular fa-arrow-right"></i></span>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// external
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";
// internal
import img_1 from "~/assets/img/slider/about/about-gallery-slider-1.jpg";
import img_2 from "~/assets/img/slider/about/about-gallery-slider-2.jpg";
import img_3 from "~/assets/img/slider/about/about-gallery-slider-3.jpg";
import img_4 from "~/assets/img/slider/about/about-gallery-slider-2.jpg";

export default {
  props:{
    el_style:{
      type:Boolean,
      default:false,
    }
  },
  components: { Carousel, Slide, Pagination, Navigation },
  data() {
    return {
      images: [img_1, img_2, img_3, img_4],
    };
  },
  methods: {
    handlePrev() {
      this.$refs.detailsSlider?.prev();
    },
    handleNext() {
      this.$refs.detailsSlider?.next();
    },
  },
};
</script>
