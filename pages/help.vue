<template>
  <div>
    <header-one :top_bar="false" :header_solid="true" :commonOffcanvas="true" />
    <help-center-area/>
    <help-center-articles/>
    <common-faq/>
    <help-center-contact/>
    <footer-six :style_2="true"/>
    <back-to-top/>
  </div>
</template>

<script>
import HeaderOne from "~~/layouts/headers/HeaderOne.vue";
import HelpCenterArea from '~~/components/help-center/HelpCenterArea.vue';
import HelpCenterArticles from '~~/components/help-center/HelpCenterArticles.vue';
import CommonFaq from '~~/components/faqs/CommonFaq.vue';
import HelpCenterContact from '~~/components/help-center/HelpCenterContact.vue';
import FooterSix from '~~/layouts/footers/FooterSix.vue';
import BackToTop from '~~/layouts/footers/component/BackToTop.vue';

export default {
  components: {
    HeaderOne,
    HelpCenterArea,
    CommonFaq,
    HelpCenterArticles,
    HelpCenterContact,
    FooterSix,
    BackToTop,
  },
  setup() {
    useHead({
      title: "Services Details - Creative Agency & Portfolio Vue Nuxt 3 Template",
    });
  },
};
</script>
