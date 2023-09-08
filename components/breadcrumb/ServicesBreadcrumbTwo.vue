<template>
  <section class="breadcrumb__area breadcrumb__style-5 p-relative include-bg pt-170 pb-110 blue-bg">
    <div class="breadcrumb__bg bg-luminosity include-bg"
    :style="{ backgroundImage: `url(${bg})` }">
    </div>
    <div class="container">
      <div class="row align-items-end">
        <div class="col-xxl-7 col-lg-7">
          <div class="breadcrumb__content breadcrumb__content-2 p-relative z-index-1">
            <span class="breadcrumb__title-pre">Services</span>
            <div class="breadcrumb__list">
              <span><a href="#">Home</a></span>
              <span class="dvdr"><i class="fa-solid fa-circle-small"></i></span>
              <span><a href="#">Business</a></span>
              <span class="dvdr"><i class="fa-solid fa-circle-small"></i></span>
              <span>Investment Trend Monitor: Top Trends in 2022 </span>
            </div>
            <h3 class="breadcrumb__title">Tech Solutions <br> for Business</h3>
          </div>
        </div>
        <div class="col-xxl-5 col-lg-5">
          <div class="breadcrumb__content breadcrumb__content-2 p-relative z-index-1">
            <p>Harry IT allows your business and technology computers to store, transmit, analyze, and manipulate big
              data.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import bg from '~/assets/img/breadcrumb/breadcrumb-bg-5.jpg';

export default {
  data(){
    return {bg}
  }
}
</script>
