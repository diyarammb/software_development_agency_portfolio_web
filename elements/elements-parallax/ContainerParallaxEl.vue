<template>
  <div class="elements__parallax-area pt-110 pb-120">
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Clean & Minimal Design</span>
            <h3 class="tp-section-title-3">Container Parallax</h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-xl-12">
            <div
              class="elements__parallax-item p-relative z-index-1 jarallax"
              :style="imageStyle"
            ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import bg from "~/assets/img/slider/slider-1.jpg";

export default {
  data() {
    return { bg };
  },
  computed: {
    imageStyle() {
      return {
        backgroundImage: `url(${this.bg})`,
      }
    }
  }
};
</script>

