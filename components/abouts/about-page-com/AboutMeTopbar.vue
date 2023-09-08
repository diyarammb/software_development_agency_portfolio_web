<template>
  <section
    class="about__me about__me-spacing about__me-translate include-bg"
    :style="{ backgroundImage: `url(${bg})` }"
  >
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div
            class="about__me-content"
            data-parallax='{"x": -100, "smoothness": 10}'
          >
            <h3 class="about__me-title">About Me</h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import bg from '~/assets/img/about/about-me-breadcrumb.jpg';

export default {
  data () {
    return {bg}
  }
};
</script>
