<template>
    <footer class="pt-8 pb-4 mt-8">
        <div class="max-w-screen-xl mx-auto px-4 flex flex-col md:flex-row md:justify-between md:items-start gap-8">
            <div class="flex-1 min-w-[250px]">
                <div class="flex items-center mb-2">
                    <NuxtImg src="/img/pro-m_logo.png" alt="Project C Logo" class="h-auto w-35 mr-2" />
                </div>
                <p class="text-gray-500 text-sm mb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                    Suspendisse varius enim in eros elementum tristique.</p>
                <div class="flex gap-2 mb-4">
                    <a href="#" class="p-2 rounded bg-gray-100 hover:bg-[#0075BE] hover:text-white transition">
                        <Icon name="mdi:facebook" class="text-[20px]" />
                    </a>
                    <a href="#" class="p-2 rounded bg-gray-100 hover:bg-[#0075BE] hover:text-white transition">
                        <Icon name="mdi:twitter" class="text-[20px]" />
                    </a>
                    <a href="#" class="p-2 rounded bg-gray-100 hover:bg-[#0075BE] hover:text-white transition">
                        <Icon name="mdi:instagram" class="text-[20px]" />
                    </a>
                    <a href="#" class="p-2 rounded bg-gray-100 hover:bg-[#0075BE] hover:text-white transition">
                        <Icon name="mdi:linkedin" class="text-[20px]" />
                    </a>
                    <a href="#" class="p-2 rounded bg-gray-100 hover:bg-[#0075BE] hover:text-white transition">
                        <Icon name="mdi:youtube" class="text-[20px]" />
                    </a>
                </div>
            </div>
            <div class="flex-1 min-w-[300px] flex flex-col items-start md:items-end">
                <form class="flex w-full max-w-md mb-2">
                    <input type="email" placeholder="Enter your email"
                        class="flex-1 px-4 py-2 border border-gray-300 rounded-l-lg focus:outline-none" />
                    <button type="submit"
                        class="px-6 py-2 bg-[#0075BE] text-white rounded-r-lg font-medium hover:bg-[#0075BE] transition">Subscribe</button>
                </form>
                <div class="text-xs text-gray-400">By clicking Subscribe you’re confirming that you agree with our <a
                        href="#" class="underline">Terms and Conditions</a>.</div>
            </div>
        </div>
        <div
            class="max-w-screen-xl mx-auto px-4 mt-8 border-t border-gray-200 pt-4 flex flex-col md:flex-row justify-between items-center text-xs text-gray-500">
            <div class="mb-2 md:mb-0">
                <a href="#" class="hover:underline">Cookies Settings</a> | <a href="#" class="hover:underline">Terms and
                    Conditions</a> | <a href="#" class="hover:underline">Privacy Policy</a>
            </div>
        </div>
    </footer>
</template>

<script setup lang="ts">
</script>

<style scoped></style>
