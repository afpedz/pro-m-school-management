<template>
    <section class="max-w-screen-xl mx-auto text-center py-4">
        <h2 class="text-2xl font-bold text-gray-800 mb-6">What our <span class="text-[#0075BE]">Clients</span> say!</h2>
        <div class="grid grid-cols-9 gap-4 text-gray-600 pb-8">
            <div class="col-span-5 col-start-3 font-light text-gray-500">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum
                tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla, ut commodo diam libero vitae
                erat.
            </div>
        </div>

        <div class="flex flex-row gap-16">
            <div v-for="(testimonial, idx) in testimonials" :key="idx"
                class="flex flex-col justify-center items-center w-1/2">
                <NuxtImg class="h-[90px] w-auto pb-4" :src="testimonial.img" alt="logo" />
                <div class="text-medium text-black text-center py-4">
                    {{ testimonial.text }}
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const testimonials = [
    {
        img: '/img/pro-m_logo.png',
        text: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla, ut commodo diam libero vitae erat."'
    },
    {
        img: '/img/pro-m_logo.png',
        text: '"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla, ut commodo diam libero vitae erat."'
    }
]
</script>

<style scoped></style>