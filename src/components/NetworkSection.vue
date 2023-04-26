<script>
export default {
    name: 'NetworkSection'

}
</script>

<template>
      <section class="network">
         <div class="container d-flex">
            <div class="left w-50">
               <h6 class="text-uppercase color_dg fw-bold">about the network</h6>
               <h3 class="fw-bolder text-white"><span class="bg_dg rounded-2 px-2">The</span> Company</h3>
               <p class="text-white my-3">For 12 years we have been providing audit and warranty, financial advice, risk advice, taxes and related services to select clients.</p>
               <div class="cont_cards d-flex flex-wrap">
                  <div class="net_card w-50">
                     <span class="fw-bold text-white">Tradition</span>
                     <p class="text_grey">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="net_card w-50">
                     <span class="fw-bold text-white">Security</span>
                     <p class="text_grey">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="net_card w-50">
                     <span class="fw-bold text-white">Certificate</span>
                     <p class="text_grey">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                  </div>
                  <div class="net_card w-50">
                     <span class="fw-bold text-white">Expertise</span>
                     <p class="text_grey">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                  </div>
               </div>
               <button class="btn text-uppercase mx-2 text-white bg_dg">get in touch</button>
               <button class="btn text-uppercase mx-2 text-white">read more</button>
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
.network {
      background-color: $bg-network;
      background-image: url('/images/about-4.jpg');
      background-position:  right ;
      background-size: 50%;
      background-repeat:no-repeat;
      padding: 8rem 0;
   }
   .container {
      width:70%;

      .left button:last-child {
         border: 1px solid $dark-green;
      }
   }
</style>