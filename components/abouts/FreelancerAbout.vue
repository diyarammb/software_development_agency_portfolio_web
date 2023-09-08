<template>
  <section id="about" class="about__area pt-80 pb-120 grey-bg-7">
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="section__title-wrapper-2 text-center mb-40">
            <span class="section__title-pre-2">INTRODUCTION</span>
            <h3 class="section__title-2">about me</h3>
            <p>A brand today is all about how it makes your customers feel.</p>
          </div>
        </div>
      </div>
      <!-- counter area start -->
      <freelancer-counter/>
      <!-- counter area end -->
      <div class="row justify-content-center">
        <div class="col-xxl-8 col-xl-8 col-lg-10">
          <div
            class="about__author-wrapper text-center"
            data-sal="slide-up" data-sal-delay="130" data-sal-duration="1000"
          >
            <div class="about__author-text">
              <p>
                Im a UX Designer, Over the past 10+ years I’ve created
                well-crafted mobile and web apps by connecting Business goals
                with user needs.Currently Service and Interaction Designer
                UIUXer office.
              </p>
            </div>
            <div class="about__author-info">
              <h3 class="about__author-title-2">Douglas Lyphe</h3>
              <div class="about__author-sign">
                <img src="~/assets/img/about/about-author-sign.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import FreelancerCounter from '../counters/FreelancerCounter.vue';
import SalScrollAnimationMixin from '~/mixins/SalScrollAnimationMixin';

export default {
  mixins:[SalScrollAnimationMixin],
  components:{FreelancerCounter}
};
</script>
