<template>
    <div>
        <UCarousel v-slot="{ item }" :items="items" :ui="{ item: 'flex-shrink-0 basis-1/6' }"
            :autoplay="{ delay: 2000 }" class="w-full">
            <div class="flex flex-col items-center mx-2">
                <img :src="item.avatar.src" :alt="item.name" class="rounded-full w-24 h-24 object-cover mb-2 shadow-lg">
                <p class="font-semibold text-lg">{{ item.name }}</p>
                <p class="text-sm text-gray-600">UI / UX Designer</p>
            </div>
        </UCarousel>
    </div>
</template>

<script lang="ts" setup>
const items = [{
    name: 'Sébastien Chopin',
    to: 'https://github.com/Atinux',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/atinux' }
}, {
    name: 'Sébastien Chopin',
    to: 'https://github.com/Atinux',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/atinux' }
},
{
    name: 'Sébastien Chopin',
    to: 'https://github.com/Atinux',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/atinux' }
},
{
    name: 'Sébastien Chopin',
    to: 'https://github.com/Atinux',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/atinux' }
},
{
    name: 'Sébastien Chopin',
    to: 'https://github.com/Atinux',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/atinux' }
}, {
    name: 'Pooya Parsa',
    to: 'https://github.com/pi0',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/pi0' }
}, {
    name: 'Daniel Roe',
    to: 'https://github.com/danielroe',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/danielroe' }
}, {
    name: 'Anthony Fu',
    to: 'https://github.com/antfu',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/antfu' },
},
{
    name: 'Anthony Fu',
    to: 'https://github.com/antfu',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/antfu' },

},
{
    name: 'Anthony Fu',
    to: 'https://github.com/antfu',
    avatar: { src: 'https://ipx.nuxt.com/f_auto,s_192x192/gh_avatar/antfu' },

}]
</script>

<style></style>