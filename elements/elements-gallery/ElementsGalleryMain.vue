<template>
  <common-breadcrumb
    title="Have a look to our Gallery Style"
    subtitle="Elements"
  />
  <el-gallery-style-one />
  <home-portfolio />
  <el-gallery-style-two />
  <el-gallery-style-three />
  <creative-portfolio/>
  <el-gallery-style-four/>
  <el-gallery-style-five/>
  <el-gallery-style-six/>
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";
import CreativePortfolio from '~~/components/portfolios/CreativePortfolio.vue';
import HomePortfolio from "~~/components/portfolios/HomePortfolio.vue";
import ElGalleryStyleFive from './ElGalleryStyleFive.vue';
import ElGalleryStyleFour from './ElGalleryStyleFour.vue';
import ElGalleryStyleOne from "./ElGalleryStyleOne.vue";
import ElGalleryStyleSix from './ElGalleryStyleSix.vue';
import ElGalleryStyleThree from "./ElGalleryStyleThree.vue";
import ElGalleryStyleTwo from "./ElGalleryStyleTwo.vue";

export default {
  components: {
    CommonBreadcrumb,
    ElGalleryStyleOne,
    HomePortfolio,
    ElGalleryStyleTwo,
    ElGalleryStyleThree,
    CreativePortfolio,
    ElGalleryStyleFour,
    ElGalleryStyleFive,
    ElGalleryStyleSix,
  },
};
</script>
