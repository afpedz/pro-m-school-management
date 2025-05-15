<template>
    <section
        class="max-w-screen-xl mx-auto flex flex-col md:flex-row items-center justify-between gap-10 relative overflow-hidden">

        <div class="flex-1 max-w-xl z-10">
            <div class="flex items-center mb-2">
                <span class="block w-12 h-1 bg-black mr-3"></span>
                <span class="text-lg font-semibold tracking-widest text-gray-700">WHY TO CHOOSE US</span>
            </div>
            <h2 class="text-4xl md:text-5xl font-bold mb-4 leading-tight">Custom I.T Solution for Your School Business
            </h2>
            <p class="text-gray-600 mb-8">
                Our team is composed of experienced and skilled professionals from the academe, information technology,
                and other relevant fields. We are committed to helping you streamline and optimize your academic
                processes through our advanced school management system software.
            </p>
            <button
                class="mx-auto block bg-[#0075BE] text-white px-10 py-2 rounded-lg font-medium text-lg shadow hover:bg-[#005fa3] transition">Join
                Now</button>
        </div>

        <div
            class="flex-1 grid grid-cols-1 md:grid-cols-2 grid-rows-3 gap-8 relative mt-12 md:mt-0 justify-items-center">
            <Card v-for="i in 6" :key="i" title="High Quality Software"
                description="Lorem ipsum dolor sit amet consecte tur adipiscing elit semper dalaracc lacus vel facilisis."
                icon="mdi-speedometer" class="max-w-xs"
                :bgClass="[1, 4, 5].includes(i) ? 'bg-gradient-to-b from-[#2176ae] to-[#1a5276]' : 'bg-white'"
                :textClass="[1, 4, 5].includes(i) ? 'text-white' : 'text-[#2176ae]'" />
        </div>
    </section>
</template>

<script setup>
import Card from '~/components/Card.vue';
</script>

<style scoped>
/* Optional: Add custom styles for responsiveness or background icons if needed */
</style>
