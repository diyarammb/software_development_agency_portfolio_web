<template>
  <div class="instagram__slider pt-120 pb-110 box-plr-15">
    <div class="container-fluid">
      <div class="row">
        <div class="col-xxl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
            <h3 class="tp-section-title-3">Instagram Slider Style</h3>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-xxl-12">
          <slider-instagram />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SliderInstagram from "~~/components/instagram/SliderInstagram.vue";

export default {
  components: { SliderInstagram },
};
</script>
