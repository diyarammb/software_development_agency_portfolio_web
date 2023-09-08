<template>
  <footer>
    <div
      :class="`footer__area footer__style-${style_2?'blue':'green'} include-bg bg-luminosity`"
      :data-bg-color="`footer-bg-${style_2?'blue':'green-dark'}`"
      :style="{ backgroundImage: `url(${bg_shape})` }"
    >
      <div class="footer__top footer__top-7">
        <div class="container">
          <div class="row">
            <div class="col-xxl-3 col-xl-3 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget footer__widget-7 mb-50 footer-col-7-1">
                <div class="footer__logo">
                  <NuxtLink to="/">
                    <img src="~/assets/img/logo/logo.svg" alt="footer__logo" />
                  </NuxtLink>
                </div>

                <div class="footer__widget-content">
                  <div class="footer__info">
                    <p>
                      The home and elements needed to create beautiful products.
                    </p>

                    <div class="footer__contact">
                      <div class="footer__contact-call">
                        <span>
                          <a href="tel:624-423-26-72">
                            <i class="fa-solid fa-phone"></i> +624 423 26 72
                          </a>
                          </span>
                      </div>
                      <div class="footer__contact-mail">
                        <span>
                          <a href="mailto:support@harry.com">
                            support@harry.com
                          </a>
                          </span>
                      </div>
                    </div>
                    <div class="footer__social">
                      <social/>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-xxl-3 col-xl-3 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget footer__widget-7 mb-50 footer-col-7-2">
                <h3 class="footer__widget-title-7">Quick Link</h3>

                <div class="footer__widget-content">
                  <ul>
                    <li><nuxt-link href="/home-startup">Home</nuxt-link></li>
                    <li><nuxt-link href="/about">About</nuxt-link></li>
                    <li><nuxt-link href="/services">Service</nuxt-link></li>
                    <li><nuxt-link href="/portfolio-2">Portfoilo</nuxt-link></li>
                    <li><nuxt-link href="/blog">News</nuxt-link></li>
                    <li><nuxt-link href="/contact">Contact</nuxt-link></li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-xxl-2 col-xl-2 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget footer__widget-7 mb-50 footer-col-7-3">
                <h3 class="footer__widget-title-7">Resources</h3>

                <div class="footer__widget-content">
                  <ul>
                    <li><nuxt-link href="/job">Careers</nuxt-link></li>
                    <li><nuxt-link href="/job">Job Post</nuxt-link></li>
                    <li><nuxt-link href="/portfolio-2">Case Studies</nuxt-link></li>
                    <li><nuxt-link href="/help">Need Help</nuxt-link></li>
                    <li><nuxt-link href="/register">Register</nuxt-link></li>
                    <li><nuxt-link href="/404">Error 404</nuxt-link></li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-xxl-4 col-xl-4 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget footer__widget-7 mb-50 footer-col-7-4">
                <h3 class="footer__widget-title-7">Newsletter</h3>

                <div class="footer__widget-content">
                  <div class="footer__subscribe-7">
                    <p>
                      Subscribe our newsletter to get the latest news & updates.
                    </p>
                    <form @submit.prevent="handleSubmit">
                      <div class="footer__subscribe-input-7">
                        <input
                          v-model="formVal"
                          type="email"
                          placeholder="email@example.com..."
                        />
                        <button type="submit">
                          <i class="fa-regular fa-arrow-up-right"></i>
                        </button>
                      </div>
                    </form>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="footer__bottom-7">
        <div class="container">
          <div class="footer__bottom-inner-7">
            <div class="row">
              <div class="col-md-4 col-sm-6">
                <div class="footer__link-7">
                  <nuxt-link href="/policy">Privacy Policy</nuxt-link>
                  <nuxt-link href="/terms">Terms of Use</nuxt-link>
                </div>
              </div>
              <div class="col-md-4 col-sm-6">
                <div class="footer__copyright-7 text-sm-center">
                  <p>
                    <nuxt-link href="/">© {{ new Date().getFullYear() }} Harry</nuxt-link> 
                    All Rights Reserved.
                  </p>
                </div>
              </div>
              <div class="col-md-4">
                <div
                  class="footer__lang d-flex align-items-center justify-content-md-end"
                >
                  <div class="footer__lang-img mr-15">
                    <img
                      src="~/assets/img/footer/footer-lang-flag-1.png"
                      alt="footer__lang-img"
                    />
                  </div>
                  <div class="footer__lang-wrapper">
                    <span
                      @click="handleToggle"
                      class="footer__lang-selected-lang tp-lang-toggle-2"
                      id="tp-footer-lang-toggle"
                      >English</span
                    >
                    <ul :class="`footer__lang-list tp-lang-list-2 ${open?'tp-lang-list-open-2':''}`">
                      <li>Spanish</li>
                      <li>Portugese</li>
                      <li>American</li>
                      <li>Canada</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import Social from '~~/components/social/Social.vue';
import bg_shape from '~/assets/img/footer/footer-shape-3.png';

export default {
  components:{Social},
  props:{
    style_2:{
      type:Boolean,
      default:false,
    }
  },
  data(){
    return {
      bg_shape,
      open:false,
      formVal:'',
    }
  },
  methods:{
    handleToggle() {
      this.open = !this.open
    },
    handleSubmit () {
      console.log(this.formVal)
      this.formVal = ''
    }
  }
};
</script>

Social