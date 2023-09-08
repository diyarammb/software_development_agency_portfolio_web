<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <el-skill-main/>
    <Footer />
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ElSkillMain from '~~/elements/elements-skills/ElSkillMain.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import Footer from "~~/layouts/footers/Footer.vue";

export default {
  components: {
    HeaderOne,
    ElSkillMain,
    Footer,
    BackToTop,
  },
  setup() {
    useHead({
      title:
        "Element Skill - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
