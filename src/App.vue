<script>
import PageHeader from './components/PageHeader.vue'
import PageMain from './components/PageMain.vue'

export default {
   components: {
      PageHeader,
      PageMain
   },
   data() {
      return {

      }
   }
}
</script>

<template>
   <PageHeader />
   <PageMain />

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

</style>