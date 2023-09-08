<template>
  <section class="about__text pt-115 pb-100">
    <div class="container">
      <div class="row">
        <div class="col-xl-4 col-lg-4">
          <div
            class="about__text-wrapper"
            data-sal="slide-up" data-sal-delay="130" data-sal-duration="1000"
          >
            <h3 class="about__text-title">
              It started with a <br />
              bang now we're here.
            </h3>
          </div>
        </div>
        <div class="col-xl-8 col-lg-8">
          <div
            class="about__text"
            data-sal="slide-up" data-sal-delay="160" data-sal-duration="1000"
          >
            <p>
              Ut at maximus magna. Vestibulum interdum sapien in facilisis
              imperdiet. Pellentesque habitant morbi tristique senectus et netus
              et malesuada fames ac turpis egestas. Proin ac placerat risus.
              Nullam eget tortor felis. Nulla facilisi.Vestibulum mattis diam
              non luctus elementum. Cras sollicitudin, nisi in semper viverra,
              felis diam consequat mi, quis tincidunt ligula
            </p>

            <p>
              Nam nibh diam, varius quis lectus eget, laoreet cursus metus.
              morbi augue lectus, dapibus eget justo nec, consectetur auctor nis
              luctus neque.!
            </p>
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
