<script>
export default {
   data() {
      return {
         navMenu: ['home', 'services', 'about', 'projects', 'results'],
         messageJumbo: 'No matter what your company needs, we will be ready to assist you in the best possible way.'
      }
   }
}
</script>

<template>
   <!-- Header -->
   <header>
      <div class="container_info d-flex justify-content-between p-2">
         <div class="info">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
               class="bi bi-clock-fill me-2" viewBox="0 0 16 16">
               <path
                  d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zM8 3.5a.5.5 0 0 0-1 0V9a.5.5 0 0 0 .252.434l3.5 2a.5.5 0 0 0 .496-.868L8 8.71V3.5z" />
            </svg>
            <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
         </div>
         <div class="contacts">
            <span class="phone">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                  class="bi bi-telephone-fill" viewBox="0 0 16 16">
                  <path fill-rule="evenodd"
                     d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
               </svg>
               +1 (305) 1234-5678</span>
            <span class="mail mx-3">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                  class="bi bi-envelope-fill" viewBox="0 0 16 16">
                  <path
                     d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
               </svg>
               hello@example.com</span>
            <span class="icons">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-facebook"
                  viewBox="0 0 16 16">
                  <path
                     d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z" />
               </svg>
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor"
                  class="bi bi-twitter mx-3" viewBox="0 0 16 16">
                  <path
                     d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z" />
               </svg>
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-linkedin"
                  viewBox="0 0 16 16">
                  <path
                     d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z" />
               </svg>
            </span>
         </div>
      </div>
      <div class="jumbotron d-flex">
         <nav class="p-2 d-flex justify-content-between">
            <div class="logo">
               <img src="/logo.PNG" alt="" class="img-fluid">
            </div>
            <div class="menu d-flex">
               <ul class="d-flex">
                  <li v-for=" option in navMenu" class="mx-3"> {{ option.toUpperCase() }}</li>   
               </ul>
               <button class="btn text-uppercase">get in touch</button>
            </div>
         </nav>
         <div class="ready_team text-center">
            <h1 class="text-dark fw-bold">Ready <span class="team px-3 rounded-2">Team</span></h1>
            <p>{{ messageJumbo }}</p>
            <button id="touch" class="btn text-uppercase mx-2">get in touch</button>
            <button id="more" class="btn text-uppercase mx-2">read more</button>
         </div>

      </div>
   </header>
   <!-- Main -->
   <main>

   </main>
   <!-- Footer -->
   <footer>

   </footer>
</template>


<style lang="scss" scoped>
@use './assets/scss/partials/variables' as *;

header {
   background-color: $header;
   color: $grey-text;

   .container_info {
      width: 70%;
      margin: auto;
   }

   .jumbotron {
      background-color: $light;
      background-image: url('/images/bg-parallax.png');
      background-position: top -90px center;
      background-size: 2700px;
      flex-direction: column;


      nav {
         width: 70%;
         margin: auto;

         ul {
            list-style: none;
         }

         li {
            cursor: pointer;
         }
         .logo {
            width: 100px;
         }

         button {
            background-color: $dark-green;
            color: $light;
         }
      }

      .ready_team {
         width:350px;
         align-self: center;

         .team {
            background-color: $light-green;
            color: $dark-green;

         }
         #touch {
            background-color: $dark-green;
            color:$light;
         }
      
         #more {
            color:$dark-green;
            border: 2px solid $dark-green;
         }
         
         
      }
   }
}
</style>