<template>
  <contact-top-area title="GET TO KNOW US" subtitle="Have a project in mind? Let’s talk."/>
  <!-- contact item start -->
  <div class="contact__item-area contact__translate-2">
    <div class="container">
        <div class="row">
          <div class="col-xl-4 col-lg-4 col-md-6">
              <div class="contact__item text-center mb-30 transition-3 white-bg">
                <div class="contact__icon">
                    <img src="~/assets/img/contact/icon/contact-icon-1.png" alt="">
                </div>
                <div class="contact__content">
                    <span class="contact-item-subtitle">Contact</span>
                    <p><a href="mailto:location@website.com">location@website.com</a></p>
                    <p><a href="tel:602-762-472-96">+(602) 762 472 96</a></p>
                </div>
              </div>
          </div>
          <div class="col-xl-4 col-lg-4 col-md-6">
              <div class="contact__item text-center mb-30 transition-3 white-bg">
                <div class="contact__icon">
                    <img src="~/assets/img/contact/icon/contact-icon-3.png" alt="">
                </div>
                <div class="contact__content">
                    <span class="contact-item-subtitle">Location</span>
                    <p><a href="https://www.google.com/maps/place/102+Thompson+St,+New+York,+NY+10012,+USA/@40.7255437,-74.004061,17z/data=!3m1!4b1!4m5!3m4!1s0x89c2598c338f691d:0x6d5f394e7a1962cc!8m2!3d40.7255397!4d-74.0018723" target="_blank">88 New South Head Rd, Triple, New York</a></p>
                </div>
              </div>
          </div>
          <div class="col-xl-4 col-lg-4 col-md-6">
              <div class="contact__item text-center mb-30 transition-3 white-bg">
                <div class="contact__icon">
                    <img src="~/assets/img/contact/icon/contact-icon-2.png" alt="">
                </div>
                <div class="contact__content">
                    <span class="contact-item-subtitle">Social Media</span>
                    <p>Follow on social media</p>
                    <div class="contact__social">
                      <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                      <a href="#"><i class="fa-brands fa-twitter"></i></a>
                      <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
                    </div>
                </div>
              </div>
          </div>
        </div>
    </div>
  </div>
  <!-- contact item end -->

  <!-- contact form start -->
  <section class="contact__form-area pt-90">
    <div class="container">
      <div class="row">
        <div class="col-xl-12">
          <div class="contact__form-2">
            <h3 class="contact__form-2-title">Send a message</h3>
            <contact-form/>
            <p class="ajax-response"></p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- contact form end -->

  <!-- contact location area start -->
  <section class="contact__location-area pb-130 pt-110">
    <div class="container">
        <div class="row">
          <div class="col-xl-5 col-lg-7 offset-xl-1 col-md-8">
              <div class="tp-section-wrapper-2 mb-35">
                <span class="tp-section-subtitle-2 subtitle-mb-9">LOCATIONS</span>
                <h3 class="tp-section-title-2 font-40">Come and visit our offices around the world</h3>
              </div>
          </div>
        </div>
        <div class="row justify-content-center">
          <div class="col-xl-10 ">
              <div class="contact__location-wrapper">
                <contact-location-item
                title="Australia Office"
                :icon="location_icon_1"
                location="contact.location@website.com"
                tel="686-324-6838"
              />
              <contact-location-item
                title="San Francisco Office"
                :icon="location_icon_2"
                location="contact.location@website.com"
                tel="686-324-6810"
              />
              <contact-location-item
                title="Egpyt Office"
                :icon="location_icon_3"
                location="contact.location@website.com"
                tel="786-324-6810"
              />
              </div>
          </div>
        </div>
    </div>
  </section>
  <!-- contact location area end -->
</template>

<script>
// internal
import ContactForm from '../forms/ContactForm.vue';
import ContactTopArea from './ContactTopArea.vue';
import location_icon_1 from "~/assets/img/contact/contact-location-1.png";
import location_icon_2 from "~/assets/img/contact/contact-location-2.png";
import location_icon_3 from "~/assets/img/contact/contact-location-3.png";
import ContactLocationItem from './ContactLocationItem.vue';

  export default {
  components: { ContactTopArea, ContactForm, ContactLocationItem },
    data () {
      return {location_icon_1,location_icon_2,location_icon_3}
    }
  }
</script>
