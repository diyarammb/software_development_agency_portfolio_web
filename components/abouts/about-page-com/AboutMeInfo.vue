<template>
  <section class="about__me-info pb-90 pt-110">
    <div class="container">
      <div class="row">
        <div class="col-xl-4 col-lg-3">
          <span class="about__me-info-subtitle">ABOUT ME</span>
        </div>
        <div class="col-xl-8 col-lg-9">
          <div
            class="about__me-info-content"
            data-sal="slide-up" data-sal-delay="130" data-sal-duration="1000"
          >
            <h4 class="about__me-info-title">
              Hi, I'm brian wilson!
              <img src="~/assets/img/about/about-me-title-icon.png" alt="" />
            </h4>
            <p>
              I'm a UX designer, prototyper, and a part-time 3D artist. I'm
              currently a Working at Fraxos, working remotely from Boston. If
              you're a creative in Boston, say hi! I love words that start with
              people, process, problem solving, paper sketches, prototyping,
              polished design, pixel-perfect products, design system, UI
              animation
            </p>

            <p>
              I’m a writer and designer working in New York City. primarily
              designs book jackets, working for Creative techs since 2000.
            </p>

            <div
              class="about__me-info-bottom d-sm-flex align-items-center mt-40"
            >
              <div class="about__me-info-btn mr-30">
                <a
                  href="https://weblearnbd.net/wp/bioxlab/wp-content/uploads/2022/09/demo-cv.pdf"
                  target="_blank"
                  class="tp-btn"
                >
                  Download CV
                  <svg
                    width="14"
                    height="14"
                    viewBox="0 0 14 14"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M1 7H13"
                      stroke="currentColor"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      d="M7 1L13 7L7 13"
                      stroke="currentColor"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </a>
              </div>
              <div class="about__me-info-social">
                <a href="#"><i class="fa-brands fa-facebook-f"></i> Facebook</a>
                <a href="#"><i class="fa-brands fa-twitter"></i> Twitter</a>
                <a href="#"><i class="fa-brands fa-linkedin-in"></i> LinkedIn</a>
              </div>
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
