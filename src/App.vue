<script>
import PageHeader from './components/PageHeader.vue'
import BusinessSection from './components/BusinessSection.vue'
import NetworkSection from './components/NetworkSection.vue'
import ProjectsSection from './components/ProjectsSection.vue'
export default {
   components: {
      PageHeader,
      BusinessSection,
      NetworkSection,
      ProjectsSection
   },
   data() {
      return {

      }
   }
}
</script>

<template>
   <PageHeader />
   <!-- Main -->
   <main class="">
      <BusinessSection/>
      <NetworkSection />
      <ProjectsSection />



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



}
</style>