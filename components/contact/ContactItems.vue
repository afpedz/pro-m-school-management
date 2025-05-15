<template>
    <section>
        <div class="max-w-screen-xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 pb-12">
            <Card v-for="(items, index) in items" :key="index" :title=items.title :description=items.description
                :icon=items.icon class="max-w-xs" bgClass='bg-white' textClass='text-black text-2xl' />
        </div>
    </section>
</template>

<script lang="ts" setup>
import Card from '../Card.vue';

const items = [
    { title: 'Visit Us', description: 'We invite you to come and explore! See what we have to offer, meet our team, and experience it all for yourself. We look forward to welcoming you!', icon: 'mdi-map-marker-radius' },
    { title: 'Call Us', description: 'We invite you to give us a call! Learn more about what we offer, connect with our team, and let us assist you. We look forward to hearing from you!', icon: 'mdi-phone' },
    { title: 'Message Us', description: 'We invite you to send us a message! Learn more about what we offer, connect with our team, and let us assist you. We look forward to chatting with you!', icon: 'mdi-message-outline' },
];


</script>

<style></style>