<template>
  <section id="tpabout" class="about__area black-bg-5 pt-170 pb-195">
    <div class="container">
      <div class="row">
        <div class="col-xl-5 col-lg-6">
          <div class="about__thumb-3 w-img wow">
            <img
              class="about-3-main-thumb wow"
              src="~/assets/img/about/3/about-1.jpg"
              alt="main-thumb"
            />
          </div>
        </div>
        <div class="col-xl-7 col-lg-6">
          <div class="about__wrapper-3 pt-20 pl-100">
            <div class="section__title-wrapper-3 mb-45">
              <span class="section__title-pre-3">01 . Read About Me</span>
              <h3 class="section__title-3 has-gradient">
                We are Best <br />
                Portrait <span>Photography</span>
              </h3>
            </div>

            <div class="about__tab">
              <div class="about__tab-nav mb-40">
                <nav>
                  <div
                    class="about__tab-inner nav tp-tab-menu d-flex flex-sm-nowrap flex-wrap"
                    id="nav-tab"
                    role="tablist"
                  >
                    <button
                      ref="active"
                      @click="handleActiveMarker"
                      class="nav-link active"
                      id="nav-self-tab"
                      data-bs-toggle="tab"
                      data-bs-target="#nav-self"
                      type="button"
                      role="tab"
                      aria-controls="nav-self"
                      aria-selected="true"
                    >
                      Myself.
                    </button>
                    <button
                      @click="handleActiveMarker"
                      class="nav-link"
                      id="nav-education-tab"
                      data-bs-toggle="tab"
                      data-bs-target="#nav-education"
                      type="button"
                      role="tab"
                      aria-controls="nav-education"
                      aria-selected="false"
                    >
                      Education.
                    </button>
                    <button
                      @click="handleActiveMarker"
                      class="nav-link"
                      id="nav-skill-tab"
                      data-bs-toggle="tab"
                      data-bs-target="#nav-skill"
                      type="button"
                      role="tab"
                      aria-controls="nav-skill"
                      aria-selected="false"
                    >
                      Main Skills.
                    </button>
                    <span
                      id="marker"
                      class="tp-tab-line d-none d-sm-inline-block"
                    ></span>
                  </div>
                </nav>
              </div>
              <div class="about__tab-content">
                <div class="tab-content" id="nav-tabContent">
                  <div
                    class="tab-pane fade show active"
                    id="nav-self"
                    role="tabpanel"
                    aria-labelledby="nav-self-tab"
                  >
                  <!-- about self start -->
                  <about-self/>
                  <!-- about self end -->
                  </div>
                  <div
                    class="tab-pane fade"
                    id="nav-education"
                    role="tabpanel"
                    aria-labelledby="nav-education-tab"
                  >
                  <!-- about-education start  -->
                  <about-education/>
                  <!-- about-education end  -->
                  </div>
                  <div
                    class="tab-pane fade"
                    id="nav-skill"
                    role="tabpanel"
                    aria-labelledby="nav-skill-tab"
                  >
                    <about-skills/>
                  </div>
                </div>
                <div class="about__btn-3 d-sm-flex">
                  <div class="about__btn-3-inner mb-20">
                    <a
                      href="https://weblearnbd.net/wp/bioxlab/wp-content/uploads/2022/09/demo-cv.pdf"
                      target="_blank"
                      class="tp-btn-2"
                      >Download CV.</a
                    >
                  </div>
                  <div class="about__btn-3-inner mb-20">
                    <nuxt-link href="/contact-2" class="tp-btn-border-3">Hire Me</nuxt-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import AboutEducation from './AboutEducation.vue';
import AboutSelf from './AboutSelf.vue';
import AboutSkills from './AboutSkills.vue';

export default {
  components: { AboutSelf, AboutEducation, AboutSkills },
  methods: {
    handleActiveMarker(e) {
      const marker = document.getElementById("marker");
      if (e.target.classList.contains("active")) {
        marker.style.left = e.target.offsetLeft + "px";
        marker.style.width = e.target.offsetWidth + "px";
      }
    },
  },
  mounted() {
    const marker = document.getElementById("marker");
    if (this.$refs.active.classList.contains("active")) {
      marker.style.left = this.$refs.active.offsetLeft + "px";
      marker.style.width = this.$refs.active.offsetWidth + "px";
    }
  },
};
</script>
