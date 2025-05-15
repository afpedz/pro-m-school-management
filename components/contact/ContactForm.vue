<template>
    <div class="max-w-screen-xl mx-auto flex flex-col md:flex-row gap-10 md:gap-16 py-8 justify-center items-start">
        <div class="bg-gray-200 p-10 md:p-12 rounded w-full md:w-[580px] min-w-[340px] flex flex-col gap-4">
            <div class="flex items-center gap-4 mb-2">
                <div class="w-16 h-1 bg-gray-900 rounded"></div>
                <h2 class="text-2xl font-semibold">Get in touch</h2>
            </div>
            <h1 class="text-4xl font-extrabold mb-2 leading-tight">Need Something?<br />Send a Message.</h1>
            <p class="text-base text-gray-900 mb-4">
                To contact us, you can fill out the form on this page and one of our team members will get back to you
                as soon as possible. Alternatively, you can reach us by phone or email using the information provided
                below.
            </p>
            <div class="flex flex-col gap-2 mt-4">
                <div class="flex items-center gap-2 text-base text-gray-900">
                    <Icon name="mdi:email-outline" class="text-lg" />
                    johndoe123@gmail.com
                </div>
                <div class="flex items-center gap-2 text-base text-gray-900">
                    <Icon name="mdi:phone-outline" class="text-lg" />
                    +63 (969) 313-6798
                </div>
                <div class="flex items-center gap-2 text-base text-gray-900">
                    <Icon name="mdi:map-marker-outline" class="text-lg" />
                    742 Evergreen Terrace<br />Springfield, OR 12345
                </div>
                <div class="flex items-center gap-2 text-base text-gray-900">
                    <Icon name="mdi:clock-outline" class="text-lg" />
                    09:00 AM - 06:00 PM
                </div>
            </div>
            <div class="mt-8 text-base">
                Looking for School Management System? <a href="#" class="text-blue-600 underline">View Full Education
                    System.</a>
            </div>
        </div>
        <form class="flex flex-col gap-4 min-w-[380px] w-full md:w-[400px] bg-white pt-6" autocomplete="off">
            <h3 class="text-xl font-semibold mb-2">Leave A Message.</h3>
            <input type="text" placeholder="Full name"
                class="px-4 py-3 border border-gray-300 rounded-lg text-base outline-none bg-gray-50 focus:border-[#0075BE] focus:ring-1 focus:ring-[#0075BE]" />
            <input type="email" placeholder="Email"
                class="px-4 py-3 border border-gray-300 rounded-lg text-base outline-none bg-gray-50 focus:border-[#0075BE] focus:ring-1 focus:ring-[#0075BE]" />
            <input type="text" placeholder="Phone"
                class="px-4 py-3 border border-gray-300 rounded-lg text-base outline-none bg-gray-50 focus:border-[#0075BE] focus:ring-1 focus:ring-[#0075BE]" />
            <input type="text" placeholder="School Name"
                class="px-4 py-3 border border-gray-300 rounded-lg text-base outline-none bg-gray-50 focus:border-[#0075BE] focus:ring-1 focus:ring-[#0075BE]" />
            <textarea placeholder="Message"
                class="min-h-[120px] px-4 py-3 border border-gray-300 rounded-lg text-base outline-none bg-gray-50 resize-y focus:border-[#0075BE] focus:ring-1 focus:ring-[#0075BE]"></textarea>
            <button type="submit"
                class="bg-[#0075BE] hover:bg-[#0076BE] text-white rounded-lg py-3 text-lg font-medium cursor-pointer mt-2 transition-colors">Submit</button>
        </form>
    </div>
</template>

<script setup lang="ts">
// No logic for now, just UI
</script>

<!-- TailwindCSS is used for all styling -->
