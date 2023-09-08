<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <team-breadcrumb
      title="We’ve Most Talented Team Members"
      subtitle="Team Members"
    />
    <team-area />
    <job-area/>
    <footer-six :style_2="true" />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import TeamBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import TeamArea from "~~/components/teams/TeamArea.vue";
import JobArea from '~~/components/job-position/JobArea.vue';
import FooterSix from "~~/layouts/footers/FooterSix.vue";
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    TeamBreadcrumb,
    TeamArea,
    FooterSix,
    JobArea,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Team - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
