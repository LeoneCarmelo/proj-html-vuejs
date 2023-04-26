<script>
import PageHeader from './components/PageHeader.vue'
export default {
   components: {
      PageHeader
   },
   data() {
      return {

      }
   }
}
</script>

<template>
<PageHeader/>
   <!-- Main -->
   <main>
      <section class="container">
         <div class="row">
            <h6 class="text-uppercase pt-5 color_dg">our business areas</h6>
            <h3 class="fw-bold">Excellence in <span class="bg_lg color_dg px-2 fw-bolder rounded-2">Services</span></h3>
            <p class="text_grey">We are leaders in providing consultancy services with a set of cutting-edge technologies
               and a team of experienced and renowned professionals. These are some options that you can hire</p>
            <a class="text-uppercase bg_dg text-light text-center rounded-2 ms-5">see all</a>
         </div>
      </section>
   </main>
   <!-- Footer -->
   <footer>

   </footer>
</template>


<style lang="scss" scoped>
@use './assets/scss/partials/variables' as *;

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




main {
   background-color: $bg-business;

   section.container {
      width: 70%;

      p {
         width:700px;
      }

      a {
         width: 100px;
         text-decoration: none;
         height: 50px;
         line-height: 45px;
         cursor: pointer;
      }
   }
}
</style>