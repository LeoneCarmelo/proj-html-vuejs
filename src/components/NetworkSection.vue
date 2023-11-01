<script>
export default {
   name: 'NetworkSection'

}
</script>

<template>
   <section class="network">
      <div class="bullets_up d-flex">
         <!--            <img src="/bullets.png" alt="" class="img-fluid"> -->
      </div>
      <div class="container d-flex">
         <div class="left w-50 pt-4">
            <h6 class="text-uppercase color_dg fw-bold">about the network</h6>
            <h3 class="fw-bolder text-white"><span class="darker_g rounded-2 px-2">The</span> Company</h3>
            <p class="text-white my-3">For 12 years we have been providing audit and warranty, financial advice, risk
               advice, taxes and related services to select clients.</p>
            <div class="cont_cards d-flex flex-wrap justify-content-center align-items-center">
               <div class="net_card w-50 py-3 pe-3">
                  <img src="/medal.png" alt="">
                  <span class="fw-bold text-white ms-1 d-block">Tradition</span>
                  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
               </div>
               <div class="net_card w-50 py-3 pe-3">
                  <img src="/lock.png" alt="">
                  <span class="fw-bold text-white ms-1 d-block">Security</span>
                  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
               </div>
               <div class="net_card w-50 py-3 pe-3">
                  <img src="/pencil.png" alt="">
                  <span class="fw-bold text-white ms-1 d-block">Certificate</span>
                  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
               </div>
               <div class="net_card w-50 py-3 pe-3">
                  <img src="/hat.png" alt="">
                  <span class="fw-bold text-white ms-1 d-block">Expertise</span>
                  <p class="pt-1">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
               </div>
            </div>
            <div class="d-flex justify-content-center align-items-center gap-2">
               <button class="btn text-uppercase mx-2 text-white bg_dg">get in touch</button>
               <button id="read" class="btn text-uppercase mx-2 text-white">read more</button>
            </div>
         </div>
      </div>
      <div class="bullets_down d-flex">
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

.darker_g {
   background-color: $darker-green;
}

/* #endregion Utility */
.network {
   background-color: $bg-network;
   background-image: url('/images/about-4.jpg');
   background-position: right;
   background-size: 50%;
   background-repeat: no-repeat;
   padding: 7rem 0;
   position: relative;

   .net_card p {
      color: $grey-text;
   }

   .bullets_up {
      width: 100px;
      height: 45px;
      position: absolute;
      top: -25px;
      left: 46%;
      background-image: url('/bullets.png');
      background-position: center;
      background-size: cover;
      opacity: 0.5;
   }

   .bullets_down {
      width: 100px;
      height: 45px;
      position: absolute;
      bottom: -20px;
      left: 46%;
      background-image: url('/bullets.png');
      background-position: center;
      background-size: cover;
      opacity: 0.5;
   }
}

@media screen and (max-width: 768px) {
   .network {
      background-size: 100%;

      .left {
         width: auto !important;
      }

      .net_card p  {
         color: white !important;
      }
   }
}

.container {
   width: 70%;



   .left button:last-child {
      border: 1px solid $dark-green;
   }
}

#read:hover {
   background-color: $dark-green;
}</style>