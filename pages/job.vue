<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <job-section-title/>
    <job-thumb-area/>
    <job-area :style_2="true"/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import JobSectionTitle from '~~/components/job/JobSectionTitle.vue';
import JobThumbArea from '~~/components/job/JobThumbArea.vue';
import JobArea from '~~/components/job-position/JobArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    JobSectionTitle,
    JobThumbArea,
    JobArea,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Job - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
