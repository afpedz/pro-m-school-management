<template>
    <section class="relative w-full h-[400px] md:h-[500px] flex items-center justify-center">
        <NuxtImg :src="image" :alt="title" class="absolute inset-0 w-full h-full object-cover object-center z-0"
            quality="100" :placeholder="true" />
        <div
            class="absolute inset-0 z-10 bg-black/50 md:bg-gradient-to-b md:from-black/60 md:via-black/40 md:to-black/60">
        </div>
        <div class="relative z-15 flex flex-col items-center justify-center w-full h-full text-center px-4">
            <h1 class="text-4xl md:text-5xl font-bold text-white mb-4 drop-shadow-lg">
                {{ title }}
            </h1>
            <p class="text-lg md:text-xl text-white max-w-1/2 mx-auto drop-shadow">
                {{ description }}
            </p>
        </div>
    </section>
</template>

<script setup lang="ts">
const props = defineProps({
    title: { type: String, required: true },
    description: { type: String, required: true },
    image: { type: String, required: true }
});
</script>

<style scoped></style>
