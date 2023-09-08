<template>
  <common-breadcrumb
    title="Have a look to our map styles"
    subtitle="Elements"
  />
   <!-- map area start --> 
  <section class="contact__map pt-110">
    <div class="container-fluid gx-0">
      <div class="row gx-0">
        <div class="col-xl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Contact Map</span>
            <h3 class="tp-section-title-3">Classic Map</h3>
          </div>
        </div>
      </div>
      <div class="row gx-0">
        <div class="col-xl-12">
          <div class="contact__map-wrapper contact__map-height">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3023.658226631064!2d-74.0018723!3d40.7255397!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c2598c338f691d%3A0x6d5f394e7a1962cc!2s102%20Thompson%20St%2C%20New%20York%2C%20NY%2010012%2C%20USA!5e0!3m2!1sen!2sbd!4v1665805047384!5m2!1sen!2sbd"></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
    <!-- map area end --> 

  <!-- Map Black area start --> 
  <section class="contact__M pt-110 pb-120">
    <div class="container-fluid gx-0">
      <div class="row gx-0">
        <div class="col-xl-12">
          <div class="tp-section-wrapper-3 mb-60 text-center">
            <span class="tp-section-subtitle-3">Contact Map</span>
            <h3 class="tp-section-title-3">Black Color Map</h3>
          </div>
        </div>
      </div>
      <div class="row gx-0">
        <div class="col-xl-12">
          <div class="contact__map-wrapper contact__map-height contact__map-black">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3023.658226631064!2d-74.0018723!3d40.7255397!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c2598c338f691d%3A0x6d5f394e7a1962cc!2s102%20Thompson%20St%2C%20New%20York%2C%20NY%2010012%2C%20USA!5e0!3m2!1sen!2sbd!4v1665805047384!5m2!1sen!2sbd"></iframe>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Map Black area end --> 
</template>

<script>
import CommonBreadcrumb from "~~/components/breadcrumb/CommonBreadcrumb.vue";

export default {
  components: { CommonBreadcrumb },
};
</script>
