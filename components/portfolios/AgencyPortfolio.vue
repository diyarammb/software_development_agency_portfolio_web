<template>
  <section
    class="portfolio__area portfolio__overlay-5 pt-110 pb-120 p-relative z-index-1"
  >
    <div class="portfolio__shape">
      <img
        class="portfolio__shape-6"
        src="~/assets/img/portfolio/5/shape/shape-1.png"
        alt=""
      />
      <img
        class="portfolio__shape-7"
        src="~/assets/img/portfolio/5/shape/shape-2.png"
        alt=""
      />
    </div>
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="section__title-wrapper-5 mb-60 text-center">
            <span class="section__title-pre-5">SELECTED PROJECTS</span>
            <h3 class="section__title-5">Digital Case Studies.</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid g-0">
      <div class="row gx-0">
        <div class="col-xxl-12">
          <!-- agency-slider-items -->
          <agency-slider-items
            :portfolio_data="portfolio_data"
            :handleImagePopup="handleImagePopup"
          />
          <!-- agency-slider-items -->
        </div>
      </div>
    </div>
  </section>
  <!-- image popup start -->
  <image-popup
    ref="image_popup"
    :images="portfolio_data.map((item) => item.img)"
  />
  <!-- image popup end -->
</template>

<script>
// internal
import ImagePopup from "../common/modals/ImagePopup.vue";
import AgencySliderItems from "./AgencySliderItems.vue";
import agency_port_1 from "~/assets/img/portfolio/5/portfolio-1.jpg";
import agency_port_2 from "~/assets/img/portfolio/5/portfolio-2.jpg";
import agency_port_3 from "~/assets/img/portfolio/5/portfolio-3.jpg";
import agency_port_4 from "~/assets/img/portfolio/5/portfolio-4.jpg";
import agency_port_5 from "~/assets/img/portfolio/5/portfolio-5.jpg";
import agency_port_6 from "~/assets/img/portfolio/5/portfolio-6.jpg";

export default {
  components: { AgencySliderItems, ImagePopup },
  data() {
    return {
      portfolio_data: [
        {
          id: 1,
          img: agency_port_1,
          tag: "Sports",
          title: "Stadium Sports Cards",
          delay: "130",
        },
        {
          id: 2,
          img: agency_port_2,
          tag: "Branding & Digital Platforms",
          title: "Aliens do 3D Automobile",
          delay: "150",
        },
        {
          id: 3,
          img: agency_port_3,
          tag: "Branding & Identity",
          title: "Gallery Portfolio",
          delay: "170",
        },
        {
          id: 4,
          img: agency_port_4,
          tag: "Custom Print",
          title: "Artboard Studio",
          delay: "190",
        },
        {
          id: 5,
          img: agency_port_5,
          tag: "Custom Print",
          title: "Artboard Studio",
          delay: "190",
        },
        {
          id: 6,
          img: agency_port_6,
          tag: "Branding & Identity",
          title: "Gallery Portfolio",
          delay: "190",
        },
      ],
    };
  },
  methods: {
    handleImagePopup(index) {
      this.$refs.image_popup.showImg(index);
    },
  },
};
</script>
