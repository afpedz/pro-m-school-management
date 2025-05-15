<template>
    <section class="py-12 bg-white">
        <div class="max-w-screen-xl mx-auto px-4">
            <h2 class="text-3xl font-bold mb-2">Services</h2>
            <p class="text-gray-600 mb-8 max-w-screen-xl">Our school management system comes with a separate portal for
                every user role. An admin portal with full controls, separate portals for Management staff, Accountant,
                Teachers, Parents, and Students.</p>
            <h3 class="text-xl font-semibold text-center mb-8">PROJECT M Services</h3>
            <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-6">
                <div v-for="service in services" :key="service.title"
                    class="flex flex-col items-center p-6 border rounded-lg border-[#0075BE] hover:shadow-lg transition">
                    <div class="rounded-full border-2 border-[#0075BE] p-2">
                        <div class="bg-[#0075BE] rounded-full w-24 h-24 flex items-center justify-center">
                            <Icon :name="service.icon.replace('mdi ', 'mdi-')" class="text-white text-4xl" />
                        </div>
                    </div>

                    <span class="font-medium text-center mt-8 mb-4">{{ service.title }}</span>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts" setup>
const services = [
    { icon: 'mdi-account-plus', title: 'Admission' },
    { icon: 'mdi-file-document-edit', title: 'Enrollment' },
    { icon: 'mdi-school', title: 'School ELMS' },
    { icon: 'mdi-cash-multiple', title: 'Payment' },
    { icon: 'mdi-calendar-clock', title: 'Scheduling' },
    { icon: 'mdi-human-male-board', title: 'Teacher Database' },
    { icon: 'mdi-account-group', title: 'Student Database' },
    { icon: 'mdi-source-branch', title: 'Branch' },
    { icon: 'mdi-account-circle', title: 'Student Portal' },
    { icon: 'mdi-account-multiple', title: 'Parents Portal' },
    { icon: 'mdi-clipboard-check', title: 'Student Grading' },
    { icon: 'mdi-file-chart', title: 'Report Card' },
    { icon: 'mdi-account-tie', title: 'Human Resources' },
    { icon: 'mdi-cash-register', title: 'Cashier' },
    { icon: 'mdi-file-document', title: 'Report' },
];
</script>

<style scoped></style>
