<template>
  <div class="instagram__grid pb-90">
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
            <h3 class="tp-section-title-3">Instagram Grid Style</h3>
          </div>
        </div>
      </div>
      <div class="row">

        <div v-for="(item,i) in instagram_items" :key="i" class="col-xl-3 col-lg-3 col-md-4 col-sm-6">
          <div class="instagram__item w-img mb-30">
            <img :src="item.img" alt="ins img" />

            <div class="instagram__btn">
              <a
                :href="item.link"
                target="_blank"
                class="tp-instagram-btn popup-image"
                >
                <i class="fa-brands fa-instagram"></i>
                </a>
            </div>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
// internal
import inst_1 from "~/assets/img/instagram/instagram-1.jpg";
import inst_2 from "~/assets/img/instagram/instagram-2.jpg";
import inst_3 from "~/assets/img/instagram/instagram-3.jpg";
import inst_4 from "~/assets/img/instagram/instagram-4.jpg";
import inst_5 from "~/assets/img/instagram/instagram-5.jpg";
import inst_6 from "~/assets/img/instagram/instagram-6.jpg";
import inst_7 from "~/assets/img/instagram/instagram-7.jpg";
import inst_8 from "~/assets/img/instagram/instagram-8.jpg";

export default {
  data() {
    return {
      instagram_items: [
        { img: inst_1, link: "https://www.instagram.com/" },
        { img: inst_2, link: "https://www.instagram.com/" },
        { img: inst_3, link: "https://www.instagram.com/" },
        { img: inst_4, link: "https://www.instagram.com/" },
        { img: inst_5, link: "https://www.instagram.com/" },
        { img: inst_6, link: "https://www.instagram.com/" },
        { img: inst_7, link: "https://www.instagram.com/" },
        { img: inst_8, link: "https://www.instagram.com/" },
      ],
    };
  },
};
</script>
