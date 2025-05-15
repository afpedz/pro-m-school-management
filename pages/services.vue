<template>
    <MeetingHero title="About Our Software"
        description="Using the latest in information technology, our school management system software is designed to simplify the complex but necessary processes in order to successfully operate academic institutions. Our system enables school administrators to efficiently manage essential tasks, which in turn, makes them more flexible and more equipped in providing quality education to their students."
        image="/img/meeting.jpg" />
    <ServicesGrid />
    <WhyChooseUs />
    <FooterSection />
</template>

<script setup lang="ts">
import ServicesGrid from '~/components/services/ServicesGrid.vue';
import WhyChooseUs from '~/components/services/WhyChooseUs.vue';
</script>

<style scoped></style>