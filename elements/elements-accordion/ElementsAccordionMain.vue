<template>
  <common-breadcrumb title="Have a look to our accordion" subtitle="Elements" />
  <underline-accordion />
  <div class="tp-separator"></div>
  <tab-accordion />
  <about-faqs :el_style="true" />
  <accordion-squared-border />
  <!-- <common-faq padd="105" /> -->
  <div class="tp-separator"></div>
  <bordered-accordion/>
  <div class="tp-separator"></div>
  <faq-area :el_style="true"/>
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import AboutFaqs from "~~/components/faqs/AboutFaqs.vue";
import CommonFaq from "~~/components/faqs/CommonFaq.vue";
import FaqArea from '~~/components/faqs/FaqArea.vue';
import AccordionSquaredBorder from './AccordionSquaredBorder.vue';
import BorderedAccordion from './BorderedAccordion.vue';
import TabAccordion from "./TabAccordion.vue";
import UnderlineAccordion from "./UnderlineAccordion.vue";

export default {
  components: {
    CommonBreadcrumb,
    UnderlineAccordion,
    TabAccordion,
    AboutFaqs,
    CommonFaq,
    BorderedAccordion,
    FaqArea,
    AccordionSquaredBorder,
  },
};
</script>
