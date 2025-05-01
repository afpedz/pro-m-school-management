<template>
    <section v-for="(content, index) in sections" :key="index" class="bg-white py-4">
        <div class="max-w-screen-xl mx-auto px-16 flex justify-stretch items-center space-x-16">
            <div class="w-1/2" v-if="index % 2 === 0">
                <img :src="content.image" :alt="content.alt" class="w-[450px] h-auto" />
            </div>
            <div class="w-1/2">
                <h2 class="text-3xl font-bold mb-4">{{ content.title }}</h2>
                <p class="text-gray-500 mb-6">{{ content.description }}</p>
            </div>
            <div class="w-1/2" v-if="index % 2 !== 0">
                <img :src="content.image" :alt="content.alt" class="w-[450px] h-auto" />
            </div>
        </div>
    </section>
</template>

<script lang="ts" setup>
const sections = [
    {
        title: "24/7 Customer Support",
        description: `We’re here whenever you need us. Our dedicated support team is available 24/7 to assist schools,
            teachers, and administrators. Whether it’s a technical issue or a system query, get expert help in
            real-time—day or night.`,
        image: "/img/support_illustration.png",
        alt: "Customer Support Illustration",
    },
    {
        title: "Secure and Reliable Data Protection",
        description: `We prioritize the safety of your school’s data. Our system uses industry-standard encryption and
            real-time threat monitoring to ensure all student, faculty, and administrative information remains
            secure and protected from unauthorized access.`,
        image: "/img/security.png",
        alt: "Data Protection Illustration",
    },
];
</script>

<style scoped></style>