<template>
    <section class="text-black py-16">
        <div class="max-w-screen-xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8">
            <div v-for="(card, index) in cards" :key="index"
                class="rounded-lg overflow-hidden flex flex-col justify-between">
                <div>
                    <NuxtImg :src="card.image" :alt="card.title" class="w-full h-48 object-cover shadow-lg" />
                    <div class="p-6">
                        <h3 class="text-[#0075BE] text-sm font-semibold mb-2">{{ card.category }}</h3>
                        <h2 class="text-2xl font-bold mb-4">{{ card.title }}</h2>
                        <p class="text-gray-500 mb-6">{{ card.description }}</p>
                    </div>
                </div>
                <div class="flex items-center space-x-4 p-6">
                    <NuxtImg :src="card.authorImage" alt="Author" class="w-10 h-10 rounded-full" />
                    <div>
                        <p class="text-sm font-medium">{{ card.author }}</p>
                        <p class="text-sm text-gray-500">{{ card.date }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts" setup>
const cards = [
    {
        category: "Activities",
        title: "Lorem ipsum",
        description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto accusantium praesentium eius, ut atque fuga culpa, similique sequi cum eos quis dolorum.",
        image: "/img/activity.png",
        author: "Eleazar Quite",
        authorImage: "/img/author1.png",
        date: "Mar 16, 2025",
    },
    {
        category: "Announcements",
        title: "Lorem ipsum",
        description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit facilis asperiores porro quaerat doloribus, eveniet dolore. Adipisci tempora aut inventore optio animi., tempore temporibus quo laudantium.",
        image: "/img/announcement.png",
        author: "Eleazar Quite",
        authorImage: "/img/author2.png",
        date: "Mar 10, 2025",
    },
    {
        category: "Academic Resources",
        title: "Lorem ipsum",
        description: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint harum rerum voluptatem quo recusandae magni placeat saepe molestiae, sed excepturi cumque corporis perferendis hic.",
        image: "/img/resources.png",
        author: "Eleazar Quite",
        authorImage: "/img/author3.png",
        date: "Feb 12, 2025",
    },
];
</script>

<style scoped></style>