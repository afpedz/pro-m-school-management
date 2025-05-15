<template>
    <nav class="bg-white fixed w-full z-20 top-0 start-0 border-b border-transparent transition-all duration-300"
        :class="{ 'border-gray-200 shadow-md': isScrolled }">
        <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-2">
            <a href="/" class="flex items-center space-x-3 rtl:space-x-reverse">
                <NuxtImg src="/img/pro-m_logo.png" class="h-auto w-40" alt="Pro M Logo" />
            </a>
            <div class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse">
                <button type="button"
                    class="text-white border-1 bg-[#0075BE] hover:bg-white hover:border-[#0075BE] hover:text-[#0075BE] focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-2xl text-sm px-5 py-3.5 text-center ">Book
                    a Demo</button>
                <button data-collapse-toggle="navbar-sticky" type="button"
                    class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 "
                    aria-controls="navbar-sticky" aria-expanded="false">
                    <span class="sr-only">Open main menu</span>
                    <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none"
                        viewBox="0 0 17 14">
                        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M1 1h15M1 7h15M1 13h15" />
                    </svg>
                </button>
            </div>
            <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="navbar-sticky">
                <ul
                    class="flex flex-col p-4 gap-8 md:p-0 mt-4 font-medium border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white ">
                    <li>
                        <NuxtLink to="/" class="block py-2 px-3 rounded-sm md:p-0"
                            :class="{ 'text-[#0075BE]': $route.path === '/' }" aria-current="page">Home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/services" class="block py-2 px-3 rounded-sm md:p-0"
                            :class="{ 'text-[#0075BE]': $route.path === '/services' }">Services</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/about-us" class="block py-2 px-3 rounded-sm md:p-0"
                            :class="{ 'text-[#0075BE]': $route.path === '/about-us' }">About Us</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/contact-us" class="block py-2 px-3 rounded-sm md:p-0"
                            :class="{ 'text-[#0075BE]': $route.path === '/contact-us' }">Contact Us</NuxtLink>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts" setup>
import { ref, onMounted, onUnmounted } from 'vue';
import { useRoute } from 'vue-router';
import { useHead } from '#app';

const isScrolled = ref(false);

const handleScroll = () => {
    isScrolled.value = window.scrollY > 0;
};

onMounted(() => {
    window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
});

// Dynamic title logic
const route = useRoute();
const getTitle = (path: string) => {
    switch (path) {
        case '/':
            return 'Home';
        case '/services':
            return 'Services';
        case '/about-us':
            return 'About Us';
        case '/contact-us':
            return 'Contact Us';
        default:
            return 'Project M';
    }
};

useHead(() => ({
    title: getTitle(route.path)
}));
</script>

<style></style>