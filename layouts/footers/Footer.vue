<template>
  <footer>
    <div class="footer__area" data-bg-color="footer-bg">
      <div class="footer__top">
        <div class="container">
          <div class="row">
            <div class="col-xxl-3 col-xl-3 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget mb-50 footer-col-1">
                <div class="footer__logo">
                  <nuxt-link href="/">
                    <img src="~/assets/img/logo/logo.svg" alt="">
                  </nuxt-link>
                </div>
                <div class="footer__widget-content">
                  <div class="footer__info">
                    <p>The home and elements needed to create beautiful products.</p>
                    <div class="footer__contact">
                      <div class="footer__contact-call">
                        <span><a href="tel:624-423-26-72"><i class="fa-solid fa-phone"></i> +624 423 26 72</a></span>
                      </div>
                      <div class="footer__contact-mail">
                        <span><a href="mailto:support@harry.com">support@harry.com</a></span>
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
              <div class="footer__widget mb-50 footer-col-2">
                <h3 class="footer__widget-title">Quick Link</h3>
                <div class="footer__widget-content">
                  <ul>
                    <li><nuxt-link href="/">Home</nuxt-link></li>
                    <li><nuxt-link href="/about">About</nuxt-link></li>
                    <li><nuxt-link href="/services">Service</nuxt-link></li>
                    <li><a href="#">Testimonials</a></li>
                    <li><nuxt-link href="/blog-grid">News</nuxt-link></li>
                    <li><nuxt-link href="/contact">Contact</nuxt-link></li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-xxl-3 col-xl-3 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget mb-50 footer-col-3">
                <h3 class="footer__widget-title">Resources</h3>
                <div class="footer__widget-content">
                  <ul>
                    <li><nuxt-link href="/job">Careers</nuxt-link></li>
                    <li><nuxt-link href="/job">Job Post</nuxt-link></li>
                    <li><nuxt-link href="/portfolio-details">Case Studies</nuxt-link></li>
                    <li><nuxt-link href="/help">Help</nuxt-link></li>
                    <li><nuxt-link href="/register">Register</nuxt-link></li>
                    <li><nuxt-link href="/404">Error 404</nuxt-link></li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="col-xxl-3 col-xl-3 col-lg-3 col-md-6 col-sm-6">
              <div class="footer__widget mb-50 footer-col-4">
                <h3 class="footer__widget-title">Downloads</h3>
                <div class="footer__widget-content">
                  <div class="footer__app mb-30">
                    <div class="footer__app-item">
                      <a href="#" class="tp-btn-app">
                        <svg width="15" height="16" viewBox="0 0 15 16" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path
                            d="M6.72221 12.4448V14.7782C6.72221 15.206 6.3722 15.556 5.94442 15.556C5.51663 15.556 5.16663 15.206 5.16663 14.7782V12.4448H6.72221Z"
                            fill="currentColor" />
                          <path
                            d="M9.83329 12.4448V14.7782C9.83329 15.206 9.48328 15.556 9.0555 15.556C8.62772 15.556 8.27771 15.206 8.27771 14.7782V12.4448H9.83329Z"
                            fill="currentColor" />
                          <path
                            d="M11.3891 6.99992V10.8889C11.3891 11.7444 10.6891 12.4444 9.83352 12.4444H5.16679C4.31122 12.4444 3.61121 11.7444 3.61121 10.8889V6.99992C3.61121 6.14435 4.31122 5.44434 5.16679 5.44434H9.83352C10.6891 5.44434 11.3891 6.14435 11.3891 6.99992Z"
                            fill="currentColor" />
                          <path
                            d="M2.05558 6.99947V10.1106C2.05558 10.5384 1.70557 10.8884 1.27779 10.8884C0.850005 10.8884 0.5 10.5384 0.5 10.1106V6.99947C0.5 6.57169 0.850005 6.22168 1.27779 6.22168C1.70557 6.22168 2.05558 6.57169 2.05558 6.99947Z"
                            fill="currentColor" />
                          <path
                            d="M14.4999 6.99947V10.1106C14.4999 10.5384 14.1499 10.8884 13.7221 10.8884C13.2943 10.8884 12.9443 10.5384 12.9443 10.1106V6.99947C12.9443 6.57169 13.2943 6.22168 13.7221 6.22168C14.1499 6.22168 14.4999 6.57169 14.4999 6.99947Z"
                            fill="currentColor" />
                          <path
                            d="M5.63336 4.35563H9.36679C10.0512 4.35563 10.6112 3.79561 10.6112 3.11116C10.6112 1.39224 9.21899 0 7.50008 0C5.78116 0 4.38892 1.39224 4.38892 3.11116C4.38892 3.79561 4.94891 4.35563 5.63336 4.35563Z"
                            fill="currentColor" />
                        </svg>
                        Android</a>
                    </div>
                    <div class="footer__app-item">
                      <a href="#" class="tp-btn-app">
                        <svg width="13" height="17" viewBox="0 0 13 17" fill="none"
                          xmlns="http://www.w3.org/2000/svg">
                          <path fill-rule="evenodd" clip-rule="evenodd"
                            d="M9.33685 0C9.50336 0.915787 9.08709 1.83157 8.58757 2.4976C8.08805 3.16363 7.17226 3.7464 6.25648 3.66315C6.08997 2.74736 6.50624 1.91483 7.00576 1.2488C7.58853 0.582774 8.50432 0.0832534 9.33685 0ZM12.001 14.4861C12.4172 13.8201 12.667 13.4038 13 12.6545C10.4191 11.6555 10.0029 7.99232 12.5837 6.66027C11.8345 5.66123 10.7522 5.16171 9.66987 5.16171C8.92059 5.16171 8.42107 5.32822 7.92155 5.49472C7.50528 5.66123 7.17227 5.74448 6.756 5.74448C6.25648 5.74448 5.92346 5.57798 5.42394 5.41147C4.92442 5.24496 4.4249 5.07846 3.84213 5.07846C2.67658 5.07846 1.42778 5.74448 0.678502 6.99328C-0.403791 8.65835 -0.237284 11.9052 1.51104 14.5693C2.26032 15.5684 3.09285 16.6507 4.17514 16.6507C4.67466 16.6507 4.92442 16.4842 5.25744 16.4009C5.6737 16.2344 6.08997 16.0679 6.756 16.0679C7.50528 16.0679 7.83829 16.2344 8.25456 16.4009C8.58757 16.5674 8.83733 16.6507 9.33685 16.6507C10.5024 16.6507 11.3349 15.4019 12.001 14.4861Z"
                            fill="currentColor" />
                        </svg>
                        Mac iOS</a>
                    </div>
                  </div>
                  <div class="footer__qrcode d-flex align-items-center">
                    <div class="footer__qrcode-thumb mr-10">
                      <a @click.prevent="handleImagePopup(0)" class="popup-image" href="#">
                        <img src="~/assets/img/icon/qrcode.png" alt="">
                      </a>
                    </div>
                    <div class="footer__qrcode-content">
                      <p>
                        <a class="popup-image" href="~/assets/img/icon/qrcode.png">Scan to Download The Themes</a>
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="footer__bottom">
        <div class="container">
          <div class="footer__bottom-inner">
            <div class="row">
              <div class="col-sm-6">
                <div class="footer__copyright">
                  <p><nuxt-link href="/">© {{new Date().getFullYear()}} Harry</nuxt-link> 
                    All Rights Reserved.
                  </p>
                </div>
              </div>
              <div class="col-sm-6">
                <div class="footer__link text-sm-end">
                  <nuxt-link href="/policy">Privacy Policy</nuxt-link>
                  <nuxt-link href="/terms">Terms of Use</nuxt-link>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
  <!-- image popup start -->
   <image-popup ref="image_popup" :images="qrcodeImg" />
  <!-- image popup end -->
</template>

<script>
import ImagePopup from '~~/components/common/modals/ImagePopup.vue';
import Social from '~~/components/social/Social.vue';
import qrcode from '~/assets/img/icon/qrcode.png';

export default {
  components: { Social, ImagePopup },
  data () {
    return {
      qrcodeImg:[qrcode]
    }
  },
  methods:{
    handleImagePopup(index){
      this.$refs.image_popup.showImg(index);
    }
  },
  }
</script>

