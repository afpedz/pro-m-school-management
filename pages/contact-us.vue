<template>
    <div>
        <MeetingHero title="Contact Us"
            description="We’re excited for the opportunity to collaborate with you in turning your vision for educational technology into reality. Thank you for choosing Project M IT Solution as your trusted partner in education management and digital innovation."
            image="/img/meeting.jpg" />
        <ContactForm />
        <ContactItems />
        <ContactMap />
        <FooterSection />
    </div>
</template>

<script setup lang="ts">
import ContactForm from '~/components/contact/ContactForm.vue';
import ContactItems from '~/components/contact/ContactItems.vue';
import ContactMap from '~/components/contact/ContactMap.vue';

// ...
</script>

<style scoped></style>