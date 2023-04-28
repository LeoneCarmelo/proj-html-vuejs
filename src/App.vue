<script>
import PageHeader from './components/PageHeader.vue'
import PageMain from './components/PageMain.vue'
import PageFooter from './components/PageFooter.vue'

export default {
   components: {
      PageHeader,
      PageMain,
      PageFooter
   },
   data() {
      return {
         openingHours: 'Open Hours: Mon - Sat - 9:00 - 18:00',
         phoneNumber: '+1 (305) 1234-5678',
         mail: 'hello@example.com',
         address: 'Main Avenue, 987',
         contacts: {
            logo: '/logo.PNG',
            description: 'A Functional HTML Template for Corporate & Business.',
            phone: '+1 (305) 1234-5678',
            email: 'hello@example.com',
            address: 'Main Avenue, 987'
         },
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
         }
      }
   }
}
</script>

<template>
   <PageHeader :opening="openingHours" :phone="phoneNumber" :mail="mail"/>
   <PageMain />
   <PageFooter/>
</template>


<style lang="scss" scoped></style>