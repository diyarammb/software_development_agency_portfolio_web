<template>
  <portfolio-area />
  <slider-port-items />
  <skill-area />
  <agency-counter spacing="90" />
  <portfolio-images />
  <portfolio-navigation />
  <portfolio-comment-area/>
</template>

<script>
import PortfolioArea from "./PortfolioArea.vue";
import SkillArea from "./SkillArea.vue";
import SliderPortItems from "./SliderPortItems.vue";
import AgencyCounter from "~~/components/counters/AgencyCounter.vue";
import PortfolioImages from "./PortfolioImages.vue";
import PortfolioNavigation from "./PortfolioNavigation.vue";
import PortfolioCommentArea from './PortfolioCommentArea.vue';

export default {
  components: {
    PortfolioArea,
    SliderPortItems,
    SkillArea,
    AgencyCounter,
    PortfolioImages,
    PortfolioNavigation,
    PortfolioCommentArea,
  },
};
</script>
