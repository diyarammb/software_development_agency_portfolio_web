<template>
  <div>
    <header-one :top_bar="false" :commonOffcanvas="true" />
    <service-three-video/>
    <service-three-feature/>
    <service-three-about/>
    <services-three-service/>
    <services-three-testimonial/>
    <agency-brands :spacing="true"/>
    <common-faq/>
    <start-up-cta :style_2="true"/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import ServiceThreeVideo from '~~/components/video-area/ServiceThreeVideo.vue';
import ServiceThreeFeature from '~~/components/features/ServiceThreeFeature.vue';
import ServiceThreeAbout from '~~/components/abouts/ServiceThreeAbout.vue';
import ServicesThreeService from '~~/components/services/ServicesThreeService.vue';
import ServicesThreeTestimonial from '~~/components/testimonials/ServicesThreeTestimonial.vue';
import AgencyBrands from '~~/components/brands/AgencyBrands.vue';
import CommonFaq from '~~/components/faqs/CommonFaq.vue';
import StartUpCta from '~~/components/cta/StartUpCta.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    ServiceThreeVideo,
    ServiceThreeFeature,
    ServiceThreeAbout,
    ServicesThreeService,
    ServicesThreeTestimonial,
    AgencyBrands,
    CommonFaq,
    StartUpCta,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Services 3 - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
