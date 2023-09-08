<template>
 <section class="faq__area p-relative z-index-1 pt-120 pb-105">
  <div class="container">
      <div class="row">
        <div class="col-xxl-5 col-xl-5 col-lg-6">
            <div class="faq__wrapper">
              <div class="section__title-wrapper-7 mb-60">
                  <span class="section__title-pre-7">Tab Accordion</span>
                  <h3 class="section__title-7">Accordion <br> with 
                    <span class="section__title-7-highlight">
                        rounded tab
                        <svg width="240" height="22" viewBox="0 0 240 22" fill="none">
                          <path fill-rule="evenodd" clip-rule="evenodd" d="M0.440833 21.1152C78.9497 6.16225 158.05 4.53412 235.949 13.8239C237.497 14.0088 239.796 12.4065 239.988 9.93474C240.181 7.4176 238.026 5.44088 236.474 5.2332C157.99 -5.31675 79.1936 0.359501 0.316568 19.7785C-0.184784 19.9023 -0.0511379 21.2092 0.440833 21.1152Z" fill="#2CAE76"/>
                        </svg>                                 
                    </span>
                  </h3>
              </div>

              <div class="faq__tab tp-tab pr-200">
                  <nav>
                    <div class="nav nav-tabs flex-column" id="nav-tab" role="tablist">
                        <button class="nav-link active" id="nav-general-tab-2" data-bs-toggle="tab" data-bs-target="#nav-general" type="button" role="tab" aria-controls="nav-general" aria-selected="true">
                          <span>
                              <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M7.318 1.74134L2.467 5.52653C1.657 6.1574 1 7.50024 1 8.51863V15.1968C1 17.2877 2.701 19 4.789 19H15.211C17.299 19 19 17.2877 19 15.2058V8.6448C19 7.55431 18.271 6.1574 17.38 5.53554L11.818 1.63319C10.558 0.749983 8.533 0.795045 7.318 1.74134Z" stroke="#525258" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M10 15.3951V12.6914" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                              </svg>                                          
                          </span>
                          General Questions
                        </button>

                        <button class="nav-link" id="nav-community-tab-2" data-bs-toggle="tab" data-bs-target="#nav-community" type="button" role="tab" aria-controls="nav-community" aria-selected="false">
                          <span>
                              <svg width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M4 7C5.65685 7 7 5.65685 7 4C7 2.34315 5.65685 1 4 1C2.34315 1 1 2.34315 1 4C1 5.65685 2.34315 7 4 7Z" stroke="#525258" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                                <path class="icon-color-theme" d="M4 17C5.65685 17 7 15.6569 7 14C7 12.3431 5.65685 11 4 11C2.34315 11 1 12.3431 1 14C1 15.6569 2.34315 17 4 17Z" stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                                <path d="M14 17C15.6569 17 17 15.6569 17 14C17 12.3431 15.6569 11 14 11C12.3431 11 11 12.3431 11 14C11 15.6569 12.3431 17 14 17Z" stroke="#525258" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                                <path class="icon-color-theme" d="M14 7C15.6569 7 17 5.65685 17 4C17 2.34315 15.6569 1 14 1C12.3431 1 11 2.34315 11 4C11 5.65685 12.3431 7 14 7Z" stroke="currentColor" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
                              </svg>                                          
                          </span>
                          Community
                        </button>

                        <button class="nav-link" id="nav-support-tab-2" data-bs-toggle="tab" data-bs-target="#nav-support" type="button" role="tab" aria-controls="nav-support" aria-selected="false">
                          <span>
                              <svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <path d="M15.822 14.3465L16.173 17.1903C16.2629 17.9373 15.462 18.4593 14.823 18.0723L11.0522 15.8314C10.6382 15.8314 10.2332 15.8044 9.83721 15.7504C10.5032 14.9675 10.8992 13.9775 10.8992 12.9065C10.8992 10.3506 8.68525 8.28073 5.94936 8.28073C4.9054 8.28073 3.94244 8.5777 3.14148 9.09968C3.11448 8.87469 3.10547 8.64969 3.10547 8.4157C3.10547 4.32086 6.66033 1 11.0522 1C15.444 1 18.9988 4.32086 18.9988 8.4157C18.9988 10.8456 17.7479 12.9965 15.822 14.3465Z" stroke="#04121F" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                                <path class="icon-color-theme" d="M10.8996 12.907C10.8996 13.978 10.5036 14.968 9.83765 15.7509C8.94669 16.8309 7.53374 17.5238 5.9498 17.5238L3.6009 18.9188C3.20491 19.1618 2.70093 18.8288 2.75493 18.3698L2.97992 16.5969C1.77397 15.7599 1 14.419 1 12.907C1 11.3231 1.84597 9.92816 3.14192 9.10019C3.94289 8.57821 4.90584 8.28125 5.9498 8.28125C8.68569 8.28125 10.8996 10.3511 10.8996 12.907Z" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                              </svg>                                       
                          </span>
                          Support
                        </button>
                    </div>
                  </nav>
              </div>
            </div>
        </div>
        <div class="col-xxl-7 col-xl-7 col-lg-6">
            <div class="faq__tab-content tp-accordion">
              <div class="tab-content" id="nav-tabContent-2">
                  <div class="tab-pane fade show active" id="nav-general" role="tabpanel" aria-labelledby="nav-general-tab-2">
                    <div class="accordion" id="general_accordion">
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="search">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapsesearch" aria-expanded="true" aria-controls="collapsesearch">
                              Global search engine optimization
                            </button>
                          </h2>
                          <div id="collapsesearch" class="accordion-collapse collapse show" aria-labelledby="search" data-bs-parent="#general_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="social">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsesocial" aria-expanded="false" aria-controls="collapsesocial">
                              Complete Social Media Integration
                            </button>
                          </h2>
                          <div id="collapsesocial" class="accordion-collapse collapse" aria-labelledby="social" data-bs-parent="#general_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="branding">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsebranding" aria-expanded="false" aria-controls="collapsebranding">
                              Branding Strategy for startups
                            </button>
                          </h2>
                          <div id="collapsebranding" class="accordion-collapse collapse" aria-labelledby="branding" data-bs-parent="#general_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="long">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapselong" aria-expanded="false" aria-controls="collapselong">
                              How long do I get support & updates?
                            </button>
                          </h2>
                          <div id="collapselong" class="accordion-collapse collapse" aria-labelledby="long" data-bs-parent="#general_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                      </div>
                  </div>
                  <div class="tab-pane fade" id="nav-community" role="tabpanel" aria-labelledby="nav-community-tab-2">
                    <div class="accordion" id="community_accordion">
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingOne1">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne1" aria-expanded="true" aria-controls="collapseOne1">
                              What kind of marketing efforts do you specialize in?
                            </button>
                          </h2>
                          <div id="collapseOne1" class="accordion-collapse collapse show" aria-labelledby="headingOne1" data-bs-parent="#community_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingTwo2">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo2" aria-expanded="false" aria-controls="collapseTwo2">
                              What is video marketing and why do I need it?
                            </button>
                          </h2>
                          <div id="collapseTwo2" class="accordion-collapse collapse" aria-labelledby="headingTwo2" data-bs-parent="#community_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingThree2">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree2" aria-expanded="false" aria-controls="collapseThree2">
                              Does my business really need digital marketing?
                            </button>
                          </h2>
                          <div id="collapseThree2" class="accordion-collapse collapse" aria-labelledby="headingThree2" data-bs-parent="#community_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingFour2">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour2" aria-expanded="false" aria-controls="collapseFour2">
                              Do you offer startup packages?
                            </button>
                          </h2>
                          <div id="collapseFour2" class="accordion-collapse collapse" aria-labelledby="headingFour2" data-bs-parent="#community_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                      </div>
                  </div>
                  <div class="tab-pane fade" id="nav-support" role="tabpanel" aria-labelledby="nav-support-tab-2">
                    <div class="accordion" id="support_accordion">
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingOne3">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne3" aria-expanded="true" aria-controls="collapseOne3">
                              Who is the typical Curious client?
                            </button>
                          </h2>
                          <div id="collapseOne3" class="accordion-collapse collapse show" aria-labelledby="headingOne3" data-bs-parent="#support_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingTwo3">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo3" aria-expanded="false" aria-controls="collapseTwo3">
                              What are your typical timelines?
                            </button>
                          </h2>
                          <div id="collapseTwo3" class="accordion-collapse collapse" aria-labelledby="headingTwo3" data-bs-parent="#support_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingThree3">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree3" aria-expanded="false" aria-controls="collapseThree3">
                              Do you offer flexible payment terms?
                            </button>
                          </h2>
                          <div id="collapseThree3" class="accordion-collapse collapse" aria-labelledby="headingThree3" data-bs-parent="#support_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
                          </div>
                        </div>
                        <div class="accordion-item">
                          <h2 class="accordion-header" id="headingFour3">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour3" aria-expanded="false" aria-controls="collapseFour3">
                              Do you trade services for equity?
                            </button>
                          </h2>
                          <div id="collapseFour3" class="accordion-collapse collapse" aria-labelledby="headingFour3" data-bs-parent="#support_accordion">
                            <div class="accordion-body">
                              <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                            </div>
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
import TabContent from '~~/components/faqs/StartUpFaq/TabContent.vue';
import commonFaq from '~~/mixins/commonFaq';

  export default {
  components: { TabContent },
    mixins:[commonFaq]
  }
</script>
