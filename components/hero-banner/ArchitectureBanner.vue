<template>
  <section class="slider__area p-relative">
    <div class="slider__social d-none d-lg-block">
      <ul>
        <li>
          <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
        </li>
        <li>
          <a href="#" class="tw"><i class="fa-brands fa-twitter"></i></a>
        </li>
        <li>
          <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
        </li>
      </ul>
      <span>Follow Us</span>
    </div>
    <!--main slider -->
    <!-- <ClientOnly> -->
    <div class="slider__active swiper-container">
      <swiper
        :space-between="0"
        :slides-per-view="1"
        :thumbs="{ swiper: thumbsSwiper }"
        :modules="modules"
        :loop="true"
        :effect="'fade'"
        :pagination="{
          clickable: true,
          el: '.main-slider-dot-8',
          renderBullet: renderBullet,
        }"
        :navigation="{
          nextEl: '.slider-button-next, .slider-button-8-next',
          prevEl: '.slider-button-prev, .slider-button-8-prev',
        }"
      >
        <swiper-slide
          v-for="(item, i) in slider_items"
          :key="i"
          class="slider__item-8 p-relative z-index-1 slider__height-8 d-flex align-items-center"
        >
          <div
            class="slider__bg-8 include-bg"
            :style="{ backgroundImage: `url(${item.bg})` }"
          ></div>
          <div class="container">
            <div class="row justify-content-center">
              <div class="col-xxl-10 col-xl-8 col-lg-9">
                <div class="slider__content-8">
                  <h3 class="slider__title-8" v-html="item.title"></h3>
                  <p>{{ item.subtitle }}</p>

                  <div class="slider__btn-8">
                    <nuxt-link
                      href="/portfolio-details-list"
                      class="tp-btn-4 tp-style-border"
                    >
                      See Project
                      <i class="fa-regular fa-chevron-right"></i>
                    </nuxt-link>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </swiper-slide>
        <div class="main-slider-dot-8 d-none d-sm-flex"></div>
      </swiper>
    </div>
    <!-- </ClientOnly> -->

    <!-- slider__nav -->
    <div class="slider__nav d-none d-sm-block">
      <swiper
        class="slider__nav-active swiper-container"
        @swiper="setThumbsSwiper"
        :modules="modules"
        :space-between="0"
        :slides-per-view="1"
        :watch-slides-progress="true"
        :loop="true"
        :freeMode="false"
        :allow-touch-move="false"
        :navigation="{
          nextEl: '.slider-8-button-next',
          prevEl: '.slider-8-button-prev',
        }"
      >
        <swiper-slide
          v-for="(item, i) in slider_nav_items"
          :key="i"
          class="slider__nav-item d-flex align-items-center"
        >
          <div class="slider__nav-content">
            <span>{{ item.id <= 9 ? "0" : "" }}{{ item.id }}.</span>
            <h3 class="slider-nav-title" v-html="item.title"></h3>
          </div>
          <div class="slider__nav-thumb">
            <img :src="item.img" alt="image" />
          </div>
        </swiper-slide>
      </swiper>
      <div class="slider__nav-arrow d-flex flex-column">
        <button class="slider-button-8-next">
          <i class="fa-regular fa-chevron-right"></i>
        </button>
        <button class="slider-button-8-prev">
          <i class="fa-regular fa-chevron-left"></i>
        </button>
      </div>
    </div>
    <div class="mouse-scroll mouse-scroll-8">
      <a href="#tpabout" class="mouse-scroll-btn"></a>
    </div>
  </section>
</template>

<script>
// external
import { Swiper, SwiperSlide } from "swiper/vue";
import { ref } from "vue";
import {
  FreeMode,
  Thumbs,
  Controller,
  EffectFade,
  Pagination,
  Navigation,
} from "swiper";
// internal
import slider_bg_1 from "~/assets/img/slider/8/slider-1.jpg";
import slider_bg_2 from "~/assets/img/slider/8/slider-2.jpg";
import slider_bg_3 from "~/assets/img/slider/8/slider-3.jpg";
import slider_bg_4 from "~/assets/img/slider/8/slider-4.jpg";
import slider_nav_1 from "~/assets/img/slider/8/nav/slider-nav-1.jpg";
import slider_nav_2 from "~/assets/img/slider/8/nav/slider-nav-2.jpg";
import slider_nav_3 from "~/assets/img/slider/8/nav/slider-nav-3.jpg";
import slider_nav_4 from "~/assets/img/slider/8/nav/slider-nav-4.jpg";

export default {
  components:{Swiper,SwiperSlide},
  data() {
    return {
      slider_items: [
        {
          bg: slider_bg_1,
          title: `We are a fine
            <span class="slider-highlight">Architecture
              <svg width="309" height="28" viewBox="0 0 309 28" fill="none"
                  xmlns="http://www.w3.org/2000/svg">
                  <path d="M4 24C88.949 1.81947 186.908 -6.80627 304 24" stroke="#FF5A1B"
                    stroke-width="8" stroke-linecap="round" />
              </svg>
            </span>
           firm in New York`,
          subtitle:
            "Through a unique combination of engineering, construction and design disciplines and expertise.",
        },
        {
          bg: slider_bg_2,
          title: `Commercial
            <span class="slider-highlight">building
              <svg width="309" height="28" viewBox="0 0 309 28" fill="none"
                  xmlns="http://www.w3.org/2000/svg">
                  <path d="M4 24C88.949 1.81947 186.908 -6.80627 304 24" stroke="#FF5A1B"
                    stroke-width="8" stroke-linecap="round" />
              </svg>
            </span>
          Concept in village`,
          subtitle:
            "Through a unique combination of engineering, construction and design disciplines and expertise.",
        },
        {
          bg: slider_bg_3,
          title: `Premium
            <span class="slider-highlight">Real State
              <svg width="309" height="28" viewBox="0 0 309 28" fill="none"
                  xmlns="http://www.w3.org/2000/svg">
                  <path d="M4 24C88.949 1.81947 186.908 -6.80627 304 24" stroke="#FF5A1B"
                    stroke-width="8" stroke-linecap="round" />
              </svg>
            </span>
          Developers`,
          subtitle:
            "Through a unique combination of engineering, construction and design disciplines and expertise.",
        },
        {
          bg: slider_bg_4,
          title: `Preparing for
            <span class="slider-highlight">Sustainable
              <svg width="309" height="28" viewBox="0 0 309 28" fill="none"
                  xmlns="http://www.w3.org/2000/svg">
                  <path d="M4 24C88.949 1.81947 186.908 -6.80627 304 24" stroke="#FF5A1B"
                    stroke-width="8" stroke-linecap="round" />
              </svg>
            </span>
          Future Architecture`,
          subtitle:
            "Through a unique combination of engineering, construction and design disciplines and expertise.",
        },
      ],
      slider_nav_items: [
        {
          id: 1,
          title: `We are a fine Architecture <br /> firm in New York`,
          img: slider_nav_1,
        },
        {
          id: 2,
          title: `Commercial building <br /> Concept in village`,
          img: slider_nav_2,
        },
        {
          id: 3,
          title: `Commercial building <br /> Concept in village`,
          img: slider_nav_3,
        },
        {
          id: 4,
          title: `We are a fine Architecture <br /> firm in New York`,
          img: slider_nav_4,
        },
      ],
    };
  },

  methods:{
    renderBullet(index, cls) {
      return `<span class=${cls}>
                  <button>${index < 9 ? "0" : ""}${index + 1}</button>
            </span>`;
    }
  },

  setup() {
    let thumbsSwiper = ref();
    const setThumbsSwiper = (swiper) => {
      thumbsSwiper.value = swiper;
    };
    return {
      thumbsSwiper,
      setThumbsSwiper,
      modules: [
        FreeMode,
        Thumbs,
        Controller,
        EffectFade,
        Pagination,
        Navigation,
      ],
    };
  },
};
</script>
