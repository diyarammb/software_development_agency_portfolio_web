<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <about-me-topbar/>
    <about-me-info/>
    <personal-port-services :style_2="true" />
    <personal-port-skills/>
    <about-me-portfolio/>
    <about-me-testimonial/>
    <agency-brands :spacing="true" :style_2="true" />
    <about-cta/>
    <footer-six :style_2="true"/>
    <back-to-top />
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import AboutMeTopbar from '~~/components/abouts/about-page-com/AboutMeTopbar.vue';
import PersonalPortServices from "~~/components/services/PersonalPortServices.vue";
import AgencyBrands from '~~/components/brands/AgencyBrands.vue';
import AboutCta from '~~/components/cta/AboutCta.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from "~~/layouts/footers/component/BackToTop.vue";
import AboutMeInfo from '~~/components/abouts/about-page-com/AboutMeInfo.vue';
import PersonalPortSkills from '~~/components/skills/PersonalPortSkills.vue';
import AboutMePortfolio from '~~/components/abouts/about-page-com/AboutMePortfolio.vue';
import AboutMeTestimonial from '~~/components/testimonials/AboutMeTestimonial.vue';

export default {
  components: {
    HeaderOne,
    BackToTop,
    PersonalPortServices,
    AgencyBrands,
    AboutCta,
    FooterSix,
    AboutMeTopbar,
    AboutMeInfo,
    PersonalPortSkills,
    AboutMePortfolio,
    AboutMeTestimonial,
  },
  setup() {
    useHead({
      title: "About Me - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
