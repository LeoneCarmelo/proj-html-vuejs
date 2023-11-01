<script>
export default {
    name: 'NumbersSection'
}
</script>

<template>
      <section>
         <div class="numbers">
            <div class="container text-center">
               <h6 class="color_dg fw-bold text-uppercase mb-3">what we are doing</h6>
               <h3 class="fw-bolder text-white mb-5"><span class="darker_g rounded-2 px-2">Results</span> in Numbers</h3>
               <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4">
                  <div class="col mb-2">
                     <div class="result d-flex flex-column">
                        <span class="fw-bold color_dg fs-3">128</span>
                        <span class="text-white fw-bold">Certifications</span>
                     </div>
                  </div>
                  <div class="col mb-2">
                     <div class="result d-flex flex-column">
                        <span class="fw-bold color_dg fs-3">230</span>
                        <span class="text-white fw-bold">Employees</span>
                     </div>
                  </div>
                  <div class="col mb-2">
                     <div class="result d-flex flex-column">
                        <span class="fw-bold color_dg fs-3">517</span>
                        <span class="text-white fw-bold">Customers</span>
                     </div>
                  </div>
                  <div class="col mb-2">
                     <div class="result d-flex flex-column">
                        <span class="fw-bold color_dg fs-3">94</span>
                        <span class="text-white fw-bold">Countries Served</span>
                     </div>
                  </div>
               </div>
            </div>
         </div>
         <div class="logos d-flex justify-content-center mx-auto py-5 flex-wrap">
            <div class="logo m-3">
               <img src="/images/logo-4.svg" alt="" class="img-fluid">
            </div>
            <div class="logo m-3">
               <img src="/images/logo-5.svg" alt="" class="img-fluid">
            </div>
            <div class="logo m-3">
               <img src="/images/logo-1.svg" alt="" class="img-fluid">
            </div>
            <div class="logo m-3">
               <img src="/images/logo-2.svg" alt="" class="img-fluid">
            </div>
            <div class="logo m-3">
               <img src="/images/logo-3.svg" alt="" class="img-fluid">
            </div>
            <div class="logo m-3">
               <img src="/images/logo-4.svg" alt="" class="img-fluid">
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
.darker_g {
   background-color: $darker-green;
}

/* #endregion Utility */

.numbers {
      background-image: url('/images/bg-7.jpg');
      background-position: center;
      background-size: cover;
      padding: 6rem 0;

      .container {
         width: 70%;
      }
   }

   .logos {
      background-color: $bg-network;

      .logo {
         width: 70px;
      }
   }
</style>