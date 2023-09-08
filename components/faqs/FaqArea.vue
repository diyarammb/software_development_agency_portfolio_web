<template>
  <section class="faq__area pt-100 pb-25">
    <div class="container">
      <div v-if="el_style" class="row">
        <div class="col-xxl-12">
            <div class="tp-section-wrapper-3 mb-50 text-center">
              <span class="tp-section-subtitle-3">Minimal &amp; Clean Design</span>
              <h3 class="tp-section-title-3">Accordion with tab</h3>
            </div>
        </div>
      </div>
      <div class="row">
        <div class="col-xxl-12">
          <div class="faq__tab-2 tp-tab mb-50">
            <ul class="nav nav-tabs" id="myTab" role="tablist">
              <li class="nav-item" role="presentation">
                <button class="nav-link active" id="general-tab" data-bs-toggle="tab" data-bs-target="#general"
                  type="button" role="tab" aria-controls="general" aria-selected="true">
                  <span>
                    <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path opacity="0.4"
                        d="M8.1105 1.19849H6.53039C2.58011 1.19849 1 2.7786 1 6.72888V11.4692C1 15.4195 2.58011 16.9996 6.53039 16.9996H11.2707C15.221 16.9996 16.8011 15.4195 16.8011 11.4692V9.8891"
                        stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                      <path
                        d="M12.0917 2.00434L5.86607 8.22998C5.62906 8.467 5.39204 8.93313 5.34464 9.27286L5.00491 11.6509C4.8785 12.5121 5.48685 13.1125 6.34801 12.994L8.72608 12.6543C9.0579 12.6069 9.52403 12.3699 9.76895 12.1329L15.9946 5.90722C17.0691 4.83274 17.5747 3.58445 15.9946 2.00434C14.4145 0.42423 13.1662 0.929866 12.0917 2.00434Z"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path opacity="0.4" d="M11.2031 2.89703C11.7325 4.78527 13.2099 6.26267 15.106 6.79991"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    </svg>
                  </span>
                  General Questions
                </button>
              </li>
              <li class="nav-item" role="presentation">
                <button class="nav-link" id="community-tab" data-bs-toggle="tab" data-bs-target="#community" type="button"
                  role="tab" aria-controls="community" aria-selected="false">
                  <span>
                    <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path
                        d="M4 7C5.65685 7 7 5.65685 7 4C7 2.34315 5.65685 1 4 1C2.34315 1 1 2.34315 1 4C1 5.65685 2.34315 7 4 7Z"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path opacity=".4"
                        d="M4 17C5.65685 17 7 15.6569 7 14C7 12.3431 5.65685 11 4 11C2.34315 11 1 12.3431 1 14C1 15.6569 2.34315 17 4 17Z"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path
                        d="M14 17C15.6569 17 17 15.6569 17 14C17 12.3431 15.6569 11 14 11C12.3431 11 11 12.3431 11 14C11 15.6569 12.3431 17 14 17Z"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                      <path opacity=".4"
                        d="M14 7C15.6569 7 17 5.65685 17 4C17 2.34315 15.6569 1 14 1C12.3431 1 11 2.34315 11 4C11 5.65685 12.3431 7 14 7Z"
                        stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round"
                        stroke-linejoin="round" />
                    </svg>
                  </span>
                  Community
                </button>
              </li>
              <li class="nav-item" role="presentation">
                <button class="nav-link" id="support-tab" data-bs-toggle="tab" data-bs-target="#support" type="button"
                  role="tab" aria-controls="support" aria-selected="false">
                  <span>
                    <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path
                        d="M15.822 14.3465L16.173 17.1903C16.2629 17.9373 15.462 18.4593 14.823 18.0723L11.0522 15.8314C10.6382 15.8314 10.2332 15.8044 9.83721 15.7504C10.5032 14.9675 10.8992 13.9775 10.8992 12.9065C10.8992 10.3506 8.68525 8.28073 5.94936 8.28073C4.9054 8.28073 3.94244 8.5777 3.14148 9.09968C3.11448 8.87469 3.10547 8.64969 3.10547 8.4157C3.10547 4.32086 6.66033 1 11.0522 1C15.444 1 18.9988 4.32086 18.9988 8.4157C18.9988 10.8456 17.7479 12.9965 15.822 14.3465Z"
                        stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                      <path opacity=".4"
                        d="M10.8996 12.907C10.8996 13.978 10.5036 14.968 9.83765 15.7509C8.94669 16.8309 7.53374 17.5238 5.9498 17.5238L3.6009 18.9188C3.20491 19.1618 2.70093 18.8288 2.75493 18.3698L2.97992 16.5969C1.77397 15.7599 1 14.419 1 12.907C1 11.3231 1.84597 9.92816 3.14192 9.10019C3.94289 8.57821 4.90584 8.28125 5.9498 8.28125C8.68569 8.28125 10.8996 10.3511 10.8996 12.907Z"
                        stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                    </svg>
                  </span>
                  Support
                </button>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="faq__item-wrapper">

        <div class="tab-content" id="faqTabContent">

          <div v-for="(item, i) in tab_faqs" :key="i" 
          :class="`tab-pane fade ${item.active ? 'show active' : ''}`"
            :id="item.id" role="tabpanel" :aria-labelledby="`${item.id}-tab`">
            <div v-for="(faq_item, index) in item.faq_content" :key="index" class="faq__item pb-95">
              <div class="row">
                <div class="col-xl-3 col-lg-3 col-md-4">
                  <div class="faq__content">
                    <h3 class="faq__title-2" v-html="faq_item.title"></h3>
                  </div>
                </div>
                <div class="col-xl-9 col-lg-9 col-md-8">
                  <div class="faq__wrapper faq__style-4 tp-accordion">
                    <div class="accordion" :id="`${faq_item.id}-${index + 1}_accordion`">
                      <single-faq v-for="(faq, i) in faq_item.accordions" :key="i" :item="faq" />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>

        </div>

      </div>
    </div>
  </section>
</template>

<script>
import SingleFaq from './SingleFaq.vue';
export default {
  components: { SingleFaq },
  props:{
    el_style:{
      type:Boolean,
      default:false,
    }
  },
  data() {
    return {
      tab_faqs: [
        {
          id: "general",
          active: true,
          faq_content: [
            {
              id: "general",
              title: "Orders <br>& Shipping",
              accordions: [
                {
                  id: "One",
                  title: "Global search engine optimization",
                  show: true,
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-1_accordion",
                },
                {
                  id: "Two",
                  title: " Complete Social Media Integration",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-1_accordion",
                },
                {
                  id: "Three",
                  title: "Branding Strategy for startups",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-1_accordion",
                },
                {
                  id: "four",
                  title: "How long do I get support & updates?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-1_accordion",
                },
              ]
            },
            {
              id: "general",
              title: "Returns <br>& Exchanges",
              accordions: [
                {
                  id: "five",
                  title: "How do I know my package has shipped?",
                  show: true,
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-2_accordion",
                },
                {
                  id: "six",
                  title:
                    "Why are certain products unavailable to ship to Internationally?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-2_accordion",
                },
                {
                  id: "seven",
                  title: "Why is my tracking number not updating?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-2_accordion",
                },
              ]
            },
            {
              id: "general",
              title: "Discounts",
              accordions: [
                {
                  id: "eight",
                  title: "How do I know my package has shipped?",
                  show: true,
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-3_accordion",
                },
                {
                  id: "nine",
                  title:
                    "Why are certain products unavailable to ship to Internationally?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-3_accordion",
                },
                {
                  id: "ten",
                  title: "Why is my tracking number not updating?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "general-3_accordion",
                },
              ]
            },
          ],
        },
        {
          id: "community",
          faq_content: [
            {
              id: "community",
              title: "Returns <br>& Exchanges",
              accordions: [
                {
                  id: "eleven",
                  title: "Can I cancel my account at any time?",
                  show: true,
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "community-1_accordion",
                },
                {
                  id: "twelve",
                  title: "What happens after the license expires?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "community-1_accordion",
                },
                {
                  id: "thirteen",
                  title: "Does Harry have any documentations?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "community-1_accordion",
                },
                {
                  id: "fourteen",
                  title: "How long do I get support & updates?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "community-1_accordion",
                },
              ]
            },
          ],
        },
        {
          id: "support",
          faq_content: [
            {
              id: "support",
              title: "Discounts",
              accordions: [
                {
                  id: "fifteen",
                  title: "Can I cancel my account at any time?",
                  show: true,
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "support-1_accordion",
                },
                {
                  id: "sixteen",
                  title: "What happens after the license expires?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "support-1_accordion",
                },
                {
                  id: "seventeen",
                  title: "Does Harry have any documentations?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "support-1_accordion",
                },
                {
                  id: "eighteen",
                  title: "How long do I get support & updates?",
                  desc: "A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders",
                  parent: "support-1_accordion",
                },
              ]
            },
          ],
        },
      ],
    };
  },
};
</script>
