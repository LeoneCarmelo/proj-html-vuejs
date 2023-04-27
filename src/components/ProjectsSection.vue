<script>
export default {
    name: 'ProjectsSection',
    data() {
      return {
         actions: ['all', 'institutional', 'social', 'events', 'innovation', 'environment', 'technology']
      }
   }
}
</script>

<template>
      <section class="projects">
         <div class="container">
            <div class="row text-center pt-5">
               <h6 class="text-uppercase color_dg fw-bold">we do more for everyone</h6>
               <h3 class="fw-bold my-3">Actions & <span class="bg_lg color_dg px-2 rounded-2">Projects</span></h3>
               <ul class="d-flex justify-content-around text-uppercase w-75 mx-auto my-3">
                  <li class="mx-3 text_grey" v-for="action in actions">{{ action }}</li>
               </ul>
            </div>
            <div class="row row-cols-3 flex-wrap">
               <div class="col mb-4">
                  <div class="card_action ca-1 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">Academic professional program in social media</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <div class="col mb-4">
                  <div class="card_action ca-2 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">President's speech at the annual meeting</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <div class="col mb-4">
                  <div class="card_action ca-3 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">International business trip in Shanghai</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <div class="col mb-4">
                  <div class="card_action ca-4 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">Technology workshop with education theme</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <div class="col mb-4">
                  <div class="card_action ca-5 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">Donation of clothes and food to the partner NGO</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <div class="col mb-4">
                  <div class="card_action ca-6 rounded-2 p-2 text-center d-flex flex-column justify-content-end">
                     <div class="layer rounded-2"></div>
                     <h5 class="text-white fw-bold">Confraternization of the procurement team</h5>
                     <p class="text-white d-none">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
            </div>
         </div>
      </section>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

/* #region Utility */

.color_lg {
   color: $light-green
}

.color_dg {
   color: $dark-green
}

.bg_lg {
   background-color: $light-green;
}

.bg_dg {
   background-color: $dark-green;
}

.text_grey {
   color: $grey-text
}

/* #endregion Utility */

.projects{
      background-color: $light;
      padding-bottom: 7rem;

      .container {
         width: 70%;
   
         ul {
            list-style: none;
         }

         .card_action {
            width: 270px;
            height: 270px;
            background-size: cover;
            position: relative;

            .layer {
               position: absolute;
               top:0;
               left:0;
               width:inherit;
               height: inherit;
               background: #0000006d;
            }

            h5, p {
               z-index: 1;
            }
         }

         .ca-1 {
            background-image: url('/images/project-1.jpg');
         }
         .ca-2 {
            background-image: url('/images/project-2.jpg');
         }
         .ca-3 {
            background-image: url('/images/project-3.jpg');
         }
         .ca-4 {
            background-image: url('/images/project-4.jpg');
         }
         .ca-5 {
            background-image: url('/images/project-5.jpg');
         }
         .ca-6 {
            background-image: url('/images/project-6.jpg');
         }
      }
   }
</style>