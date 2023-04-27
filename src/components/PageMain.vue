<script>
import BusinessSection from './BusinessSection.vue'
import NetworkSection from './NetworkSection.vue'
import ProjectsSection from './ProjectsSection.vue'
import NumbersSection from './NumbersSection.vue'
import ActionSection from './ActionSection.vue'
export default {
    name: 'PageMain',
    components: {
        BusinessSection,
        NetworkSection,
        ProjectsSection,
        NumbersSection,
        ActionSection
    }
}
</script>

<template>
    <!-- Main -->
    <main>
        <BusinessSection />
        <NetworkSection />
        <ProjectsSection />
        <NumbersSection />
        <ActionSection />
    </main>
</template>


<style lang="scss" scoped></style>