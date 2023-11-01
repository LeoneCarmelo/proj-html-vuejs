<script>
import AboutList from './AboutList.vue'
import ServicesList from './ServicesList.vue'
import SupportList from './SupportList.vue'
import CopyRight from './CopyRight.vue'
export default {
   name: 'PageFooter',
   props: {
      logo: String,
      description: String,
      phone: String,
      email: String,
      address: String
   },
   components: {
      AboutList,
      ServicesList,
      SupportList,
      CopyRight
   },
   data() {
      return {
         aboutList: {
            name: 'About',
            list: ['The Company', 'Institutional', 'Social & Events', 'Innovation', 'Environment', 'Technology']
         },
         servicesList: {
            name: 'Services',
            list: ['Audit & Assurance', 'Financial Advisory', 'Analytic M&A', 'Middle Marketing', 'Legal Consulting', 'Regulatory Risk']
         },
         supportList: {
            name: 'Support',
            list: ['Responsability', 'Term of Use', 'About Cookies', 'Privacy Policy', 'Accessibility', 'Information']
         },
         copyright: 'Enjoy the low price. We are tracking any intention of privacy.',
         nexgen: `2020 NEXGEN is Proudly Powered by `
      }
   },
   methods:{
      scrollToTop() {
         window.scrollTo({
            top: 0,
            behavior: "smooth"
         })
      }
   }
}
</script>

<template>
   <!-- Footer -->
   <footer>
      <div class="container">
         <div class="row">
            <div class="col-12 col-md-6 col-xl-3">
               <div class="logo">
                  <img :src="logo" alt="" class="img-fluid">
               </div>
               <p class="clear_text">{{ description }}</p>
               <div class="contacts mt-4">
                  <div class="phone_number d-flex align-items-center">
                     <div class="icon">
                        <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                           class="bi bi-telephone-fill" viewBox="0 0 16 16">
                           <path fill-rule="evenodd"
                              d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
                        </svg>
                     </div>
                     <a href="#">{{ phone }}</a>
                  </div>
                  <div class="contact_email d-flex align-items-center my-3">
                     <div class="icon">
                        <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                           class="bi bi-envelope-fill" viewBox="0 0 16 16">
                           <path
                              d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
                        </svg>
                     </div>
                     <a href="#">{{ email }}</a>
                  </div>
                  <div class="address d-flex align-items-center">
                     <div class="icon">
                        <svg xmlns="http://www.w3.org/2000/svg" width="17" height="17" fill="currentColor"
                           class="bi bi-geo-alt-fill" viewBox="0 0 16 16">
                           <path
                              d="M8 16s6-5.686 6-10A6 6 0 0 0 2 6c0 4.314 6 10 6 10zm0-7a3 3 0 1 1 0-6 3 3 0 0 1 0 6z" />
                        </svg>
                     </div>
                     <a href="#">{{ address }}</a>
                  </div>
                  <button class="btn text-uppercase mx-2 text-white my-4">get in touch</button>
               </div>
            </div>
            <div class="col-12 col-md-6 col-xl-3">
               <ul>
                  <li class="py-2">{{ aboutList.name }}</li>
                  <AboutList v-for="item in aboutList.list" :list="item" />
               </ul>
            </div>
            <div class="col-12 col-md-6 col-xl-3">
               <ul>
                  <li class="py-2">{{ servicesList.name }}</li>
                  <ServicesList v-for="item in servicesList.list" :list="item" />
               </ul>
            </div>
            <div class="col-12 col-md-6 col-xl-3">
               <ul>
                  <li class="py-2">{{ supportList.name }}</li>
                  <SupportList v-for="item in supportList.list" :list="item" />
               </ul>
            </div>
         </div>
      </div>
      <CopyRight :copyright="copyright" :nexgen="nexgen"/>
      <div class="arrow" @click="scrollToTop">
         <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-arrow-up-circle"
            viewBox="0 0 16 16">
            <path fill-rule="evenodd"
               d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8zm15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-7.5 3.5a.5.5 0 0 1-1 0V5.707L5.354 7.854a.5.5 0 1 1-.708-.708l3-3a.5.5 0 0 1 .708 0l3 3a.5.5 0 0 1-.708.708L8.5 5.707V11.5z" />
         </svg>
      </div>
   </footer>
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

.clear_text {
   color: $clear-text;
}

/* #endregion Utility */

footer {
   background-color: $bg-network;
   padding: 5rem 0;
   position: relative;

   .container {
      width: 70%;

      .logo {
         width: 120px;
      }

      ul {
         list-style: none;
         color: white;
         font-weight: bold;
         background-color: $list;
         padding: 2rem 1rem;
         border-radius: 8px;
      }

      li {
         cursor: pointer;
      }

      li:hover {
         color: $dark-green;
      }

      a {
         text-decoration: none;
         color: $clear-text;
         margin-left: 0.5rem;
      }

      .icon>svg {
         fill: $clear-text
      }

      button {
         border: 1px solid $dark-green;
      }
   }



   .arrow {
      position: absolute;
      bottom: 1rem;
      right: 1rem;
      cursor: pointer;
   }
}
</style>