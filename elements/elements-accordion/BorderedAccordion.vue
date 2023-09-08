<template>
  <section class="accordion__area faq__style-3 pt-110 pb-105">
            <div class="container">
               <div class="row">
                  <div class="col-xxl-12">
                     <div class="tp-section-wrapper-3 mb-65 text-center">
                        <span class="tp-section-subtitle-3">Minimal & Clean Design</span>
                        <h3 class="tp-section-title-3">Bordered Accordion</h3>
                     </div>
                  </div>
               </div>
               <div class="row">
                  <div class="col-xl-12">
                     <div class="faq__tab-content tp-accordion">
                        <div class="accordion" id="general_accordion_p">
                           <div class="accordion-item">
                             <h2 class="accordion-header" id="headingOne_p">
                               <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne_p" aria-expanded="true" aria-controls="collapseOne_p">
                                 Can I cancel my account at any time?
                               </button>
                             </h2>
                             <div id="collapseOne_p" class="accordion-collapse collapse show" aria-labelledby="headingOne_p" data-bs-parent="#general_accordion_p">
                               <div class="accordion-body">
                                 <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                               </div>
                             </div>
                           </div>
                           <div class="accordion-item">
                             <h2 class="accordion-header" id="headingTwo_p">
                               <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo_p" aria-expanded="false" aria-controls="collapseTwo_p">
                                 What happens after the license expires?
                               </button>
                             </h2>
                             <div id="collapseTwo_p" class="accordion-collapse collapse" aria-labelledby="headingTwo_p" data-bs-parent="#general_accordion_p">
                               <div class="accordion-body">
                                 <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                               </div>
                             </div>
                           </div>
                           <div class="accordion-item">
                             <h2 class="accordion-header" id="headingThree_p">
                               <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree_p" aria-expanded="false" aria-controls="collapseThree_p">
                                 Does Harry have any documentations?
                               </button>
                             </h2>
                             <div id="collapseThree_p" class="accordion-collapse collapse" aria-labelledby="headingThree_p" data-bs-parent="#general_accordion_p">
                               <div class="accordion-body">
                                 <p>A startup or start-up is started by individual founders or entrepreneurs to search for a repeatable and scalable business model. A startup or start-up is started by individual founders...</p>
                               </div>
                             </div>
                           </div>
                           <div class="accordion-item">
                             <h2 class="accordion-header" id="headingFour_p">
                               <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour_p" aria-expanded="false" aria-controls="collapseFour_p">
                                 How long do I get support & updates?
                               </button>
                             </h2>
                             <div id="collapseFour_p" class="accordion-collapse collapse" aria-labelledby="headingFour_p" data-bs-parent="#general_accordion_p">
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
         </section>
</template>

<script>
import commonFaq from '~~/mixins/commonFaq'
  export default {
    mixins:[commonFaq]
  }
</script>
