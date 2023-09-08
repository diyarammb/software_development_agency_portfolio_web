<template>
  <div class="elements__parallax-area pt-110">
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Clean & Minimal Design</span>
            <h3 class="tp-section-title-3">Full Width Parallax</h3>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid gx-0">
      <div class="row gx-0">
        <div class="col-xl-12">
            <div
              class="elements__parallax-item p-relative z-index-1 jarallax"
              :style="{ backgroundImage: `url(${bg})` }"
            ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import bg from "~/assets/img/testimonial/4/testimonial-bg.jpg";

export default {
  data() {
    return { bg };
  },
};
</script>
