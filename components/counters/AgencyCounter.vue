<template>
  <section
    :class="`counter__area counter__border-radius pb-${spacing} p-relative z-index-1`"
  >
    <div class="counter__shape">
      <img
        class="counter__shape-11"
        src="~/assets/img/counter/5/counter-shape-1.png"
        alt="shape"
      />
      <img
        class="counter__shape-12"
        src="~/assets/img/counter/5/counter-shape-2.png"
        alt="shape"
      />
    </div>
    <div class="container">
      <div class="row">
        <div class="col-xxl-12">
          <div class="counter__info-5 text-center mb-30">
            <p>
              We completed <span>1500+</span> projects yearly successfully &
              counting
            </p>
          </div>
        </div>
      </div>
      <div class="row gx-2">
        <div
          v-for="(item, i) in counter_data"
          :key="i"
          class="col-xxl-4 col-xl-4 col-lg-4 col-md-6"
        >
          <div
            :class="`counter__item-5 counter__${item.bg} mb-30 wow zoomIn`"
            data-sal="slide-up" data-sal-delay="130" data-sal-duration="1000"
          >
            <div class="counter__icon-5">
              <span v-html="item.icon"></span>
            </div>
            <div class="counter__content-5">
              <h3 class="counter__title-5" v-html="item.title"></h3>
            </div>
            <div class="counter__no">
              <h4>
                <span class="counter">{{ item.num }}</span
                >{{ item.text }}
              </h4>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import SalScrollAnimationMixin from "~/mixins/SalScrollAnimationMixin";

export default {
  mixins: [SalScrollAnimationMixin],
  props:{
    spacing:{
      type:String,
      default:'100',
    }
  },
  data() {
    return {
      counter_data: [
        {
          delay: ".3s",
          icon: `<svg width="32" height="30" viewBox="0 0 32 30" fill="none">
              <path
                d="M9.91565 0.000244203C10.9104 0.0304958 11.8735 0.204177 12.8067 0.52154H12.8998C12.963 0.55154 13.0103 0.584697 13.0419 0.614697C13.3909 0.7268 13.7209 0.853114 14.0366 1.0268L14.6366 1.29521C14.8735 1.42153 15.1577 1.65678 15.3156 1.7531C15.4735 1.84626 15.6471 1.94257 15.7892 2.05151C17.5434 0.711011 19.6734 -0.0152929 21.8681 0.000244203C22.8644 0.000244203 23.8591 0.14102 24.8049 0.458383C30.6327 2.35309 32.7326 8.74772 30.9785 14.3371C29.9837 17.1934 28.3575 19.8002 26.2275 21.9301C23.1786 24.8827 19.8329 27.5037 16.2313 29.7616L15.8366 30L15.4261 29.7458C11.8119 27.5037 8.44725 24.8827 5.36994 21.9143C3.25418 19.7844 1.62631 17.1934 0.615805 14.3371C-1.16838 8.74772 0.93159 2.35309 6.82255 0.425226C7.28043 0.267334 7.75253 0.15681 8.22621 0.0952316H8.41568C8.85935 0.0304958 9.29987 0.000244203 9.74197 0.000244203H9.91565ZM23.9838 4.98989C23.3365 4.76726 22.626 5.1162 22.3891 5.77935C22.1681 6.44249 22.5154 7.1688 23.1786 7.40406C24.1907 7.783 24.868 8.7793 24.868 9.88296V9.93191C24.838 10.2935 24.947 10.6424 25.168 10.9108C25.3891 11.1793 25.7207 11.3356 26.068 11.3687C26.7154 11.3514 27.268 10.8319 27.3154 10.1672V9.97928C27.3627 7.76721 26.0222 5.76356 23.9838 4.98989Z"
                fill="currentColor" />
          </svg>`,
          title: "Our Global <br /> Customer",
          num: 26,
          text: "k",
          bg: "green",
        },
        {
          delay: ".5s",
          icon: `<svg width="34" height="32" viewBox="0 0 34 32" fill="none">
            <path
              d="M16.8244 0L22.0231 10.5321L33.6488 12.2313L25.2366 20.4248L27.2219 32L16.8244 26.5321L6.42692 32L8.4122 20.4248L0 12.2313L11.6257 10.5321L16.8244 0Z"
              fill="currentColor" />
          </svg>`,
          title: "Our Completed <br /> Projects",
          num: 10,
          text: "k",
          bg: "brown",
        },
        {
          delay: ".7s",
          icon: `<svg width="33" height="32" viewBox="0 0 33 32" fill="none">
            <path
              d="M11.2641 0C7.07209 0 3.66406 3.40803 3.66406 7.60007C3.66406 11.7121 6.88009 15.0401 11.0721 15.1841C11.2001 15.1681 11.3281 15.1681 11.4241 15.1841C11.4561 15.1841 11.4721 15.1841 11.5041 15.1841C11.5201 15.1841 11.5201 15.1841 11.5361 15.1841C15.6322 15.0401 18.8482 11.7121 18.8642 7.60007C18.8642 3.40803 15.4562 0 11.2641 0Z"
              fill="currentColor" />
            <path
              d="M19.3922 19.44C14.9281 16.464 7.64807 16.464 3.15203 19.44C1.12001 20.8 0 22.6401 0 24.6081C0 26.5761 1.12001 28.4001 3.13603 29.7441C5.37605 31.2481 8.32007 32.0001 11.2641 32.0001C14.2081 32.0001 17.1522 31.2481 19.3922 29.7441C21.4082 28.3841 22.5282 26.5601 22.5282 24.5761C22.5122 22.6081 21.4082 20.784 19.3922 19.44Z"
              fill="currentColor" />
            <path
              d="M28.8475 8.54411C29.1035 11.6481 26.8955 14.3682 23.8395 14.7362C23.8235 14.7362 23.8235 14.7362 23.8075 14.7362H23.7595C23.6635 14.7362 23.5675 14.7362 23.4875 14.7682C21.9355 14.8482 20.5115 14.3522 19.4395 13.4402C21.0875 11.9681 22.0315 9.76012 21.8395 7.3601C21.7275 6.06409 21.2795 4.88008 20.6075 3.87207C21.2155 3.56806 21.9195 3.37606 22.6395 3.31206C25.7755 3.04006 28.5755 5.37608 28.8475 8.54411Z"
              fill="currentColor" />
            <path
              d="M32.0482 23.344C31.9202 24.896 30.9282 26.24 29.2641 27.152C27.6641 28.0321 25.6481 28.4481 23.6481 28.4001C24.8001 27.36 25.4721 26.064 25.6001 24.688C25.7601 22.704 24.8161 20.8 22.9281 19.28C21.8561 18.432 20.6081 17.76 19.248 17.264C22.7841 16.2399 27.2321 16.928 29.9681 19.136C31.4402 20.32 32.1922 21.808 32.0482 23.344Z"
              fill="currentColor" />
          </svg>`,
          title: "Our Expert <br /> Worker",
          num: 15,
          text: "k",
          bg: "purple",
        },
      ],
    };
  },
};
</script>
