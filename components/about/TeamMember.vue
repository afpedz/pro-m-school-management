<template>
  <section class="bg-white pt-10 px-4">
    <div class="max-w-screen-xl mx-auto">
      <h2 class="text-center text-4xl font-bold mb-8">Our Professional Team</h2>
      <div class="relative">
        <div class="flex flex-wrap items-start justify-center gap-10 py-4">
          <div class="max-w-lg">
            <h1 class="text-5xl font-semibold mt-24">John Doe</h1>
            <h3 class="text-xl font-light mb-6 text-[#0075BE]">UI / UX Designer</h3>
            <p class="text-base text-gray-700 mb-6">
              Our UI/UX designer plays a pivotal role in transforming complex ideas into intuitive, user-centered
              digital
              experiences. From wireframes and user flows to high-fidelity prototypes, our designer collaborates closely
              with developers, product managers, and stakeholders to create solutions that are not only aesthetically
              pleasing but also enhance usability and accessibility. With a strong foundation in user research and
              testing, they craft experiences that align with our clients’ goals and exceed user expectations.
            </p>
            <div class="flex gap-5 text-4xl">
              <a v-for="icon in socialIcons" :key="icon.label" :href="icon.href" :aria-label="icon.label"
                :class="icon.class">
                <Icon :name="icon.iconClass.replace('mdi ', 'mdi-')" />
              </a>
            </div>
          </div>
          <div>
            <img src="/img/model.png" alt="John Doe" class="w-auto h-[820px] object-cover" />
          </div>
          <div class="absolute left-0 bottom-0 w-full flex justify-center">
            <div
              class="w-full bg-white/10 md:bg-gradient-to-b md:from-white/60 md:via-white/40 md:to-white/60 backdrop-blur-sm rounded-t-xl py-6">
              <Carousel />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
const socialIcons = [
  {
    label: 'Messenger',
    href: '#',
    iconClass: 'mdi-facebook-messenger',
    class: 'text-gray-800 hover:text-blue-500 transition-colors',
  },
  {
    label: 'LinkedIn',
    href: '#',
    iconClass: 'mdi-linkedin',
    class: 'text-gray-800 hover:text-blue-700 transition-colors',
  },
  {
    label: 'Instagram',
    href: '#',
    iconClass: 'mdi-instagram',
    class: 'text-gray-800 hover:text-pink-500 transition-colors',
  },
  {
    label: 'Facebook',
    href: '#',
    iconClass: 'mdi-facebook',
    class: 'text-gray-800 hover:text-blue-600 transition-colors',
  },
  {
    label: 'Gmail',
    href: '#',
    iconClass: 'mdi-gmail',
    class: 'text-gray-800 hover:text-red-500 transition-colors',
  },
  {
    label: 'YouTube',
    href: '#',
    iconClass: 'mdi-youtube',
    class: 'text-gray-800 hover:text-red-600 transition-colors',
  },
];


</script>