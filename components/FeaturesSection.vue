<template>
    <section class="bg-white py-16">
        <div class="max-w-screen-xl mx-auto px-16">
            <h2 class="text-3xl font-medium text-center mb-12">Project M Education I.T Solution Features</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <div v-for="(feature, index) in features" :key="index" class="text-left">
                    <div
                        class="bg-[#0075BE] text-white w-[48px] h-[48px] flex items-center justify-center rounded-lg mb-4">
                        <i :class="feature.icon"></i>
                    </div>
                    <h3 class="text-lg font-semibold mb-2">{{ feature.title }}</h3>
                    <p class="text-gray-500">{{ feature.description }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts" setup>
const features = [
    { icon: 'fas fa-hand-pointer', title: 'Friendly User', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-mobile-alt', title: 'Mobility', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-map-marker-alt', title: 'Use Anywhere', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-shield-alt', title: 'Security', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-cloud', title: 'Cloud', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-laptop-code', title: 'Easy to Deploy', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-money-bill-wave', title: 'Cost Efficient', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'fas fa-bolt', title: 'Fast Response', description: 'Get a better understanding of where your traffic is coming from.' },
];
</script>

<style></style>