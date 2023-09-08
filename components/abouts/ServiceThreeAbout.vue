<template>
  <section class="about__area pt-10 pb-130">
    <div class="container">
      <div class="row">
        <div class="col-xl-6 col-lg-6">
          <div
            class="about__thumb-15 p-relative z-index-1 w-img"
            data-sal="slide-up" data-sal-delay="130" data-sal-duration="1000"
          >
            <div class="about__thumb-15-shape">
              <img src="~/assets/img/about/15/about-thumb-shape.png" alt="shape" />
            </div>
            <img
              class="about__thumb-15-shape-2"
              src="~/assets/img/about/15/about-thumb-shape-2.png"
              alt=""
            />
            <img src="~/assets/img/about/15/about-img-1.jpg" alt="shape" />
          </div>
        </div>
        <div class="col-xl-6 col-lg-6">
          <div
            class="about__wrapper-15 pl-45"
            data-sal="slide-up" data-sal-delay="160" data-sal-duration="1000"
          >
            <div class="tp-section-wrapper-3 mb-25">
              <span class="tp-section-subtitle-3">WHAT WE DO</span>
              <h3 class="tp-section-title-3">
                World best web design service provider.
              </h3>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
            </div>
            <div class="about__list-2">
              <ul>
                <li>Art Direction</li>
                <li>Graphic Design</li>
                <li>Motion Graphics</li>
                <li>Brand Strategy</li>
                <li>Mobile App Design</li>
                <li>SEO Analytics</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SalScrollAnimationMixin from "~/mixins/SalScrollAnimationMixin";

export default {
  mixins: [SalScrollAnimationMixin],

};
</script>
