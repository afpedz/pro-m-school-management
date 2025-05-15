<template>
    <section class="bg-white py-16">
        <div class="max-w-screen-xl mx-auto px-16">
            <h2 class="text-2xl font-bold text-center mb-12">Project M Education I.T Solution Features</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-5 gap-8">
                <div v-for="(feature, index) in features" :key="index" class="text-center">
                    <Icon :name="feature.icon.replace('mdi ', 'mdi-')"
                        class="mx-auto text-[#0075BE] flex items-center justify-center text-[48px]" />
                    <h3 class="text-lg font-semibold mb-2">{{ feature.title }}</h3>
                    <p class="text-gray-500">{{ feature.description }}</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts" setup>
const features = [
    { icon: 'mdi-account', title: 'User Friendly', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-security', title: 'Security', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-map-marker-radius-outline', title: 'Use Anywhere', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-cellphone', title: 'Mobility', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-cellphone', title: 'Mobility', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-weather-cloudy', title: 'Cloud', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-desktop-classic', title: 'Easy to Deploy', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-cash-multiple', title: 'Cost Efficient', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-speedometer', title: 'Fast Response', description: 'Get a better understanding of where your traffic is coming from.' },
    { icon: 'mdi-speedometer', title: 'Fast Response', description: 'Get a better understanding of where your traffic is coming from.' },
];
</script>

<style></style>