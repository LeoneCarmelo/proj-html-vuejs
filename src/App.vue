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
         contacts: {
            logo: '/logo.PNG',
            description: 'A Functional HTML Template for Corporate & Business.',
            phone: '+1 (305) 1234-5678',
            email: 'hello@example.com',
            address: 'Main Avenue, 987'
         }
      }
   }
}
</script>

<template>
   <PageHeader :opening="openingHours" :phone="contacts.phone" :mail="contacts.email"/>
   <PageMain />
   <PageFooter :logo="contacts.logo" :description="contacts.description" :phone="contacts.phone" :email="contacts.email" :address="contacts.address"/>
</template>


<style lang="scss" scoped></style>