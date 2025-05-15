<template>
  <div :class="[
    'card flex flex-col items-center justify-center p-8 w-full h-full rounded-lg',
    bgClass,
    textClass
  ]">
    <span v-if="icon" class="mb-4 text-5xl">
      <Icon :name="icon.replace('mdi ', 'mdi-')" />
    </span>
    <h3 class="text-medium font-semibold mb-2 text-center">{{ title }}</h3>
    <p class="text-center text-xs font-light">{{ description }}</p>
  </div>
</template>

<script setup>
const props = defineProps({
  title: String,
  description: String,
  icon: String,
  bgClass: {
    type: String,
    default: 'bg-gradient-to-b from-[#2176ae] to-[#1a5276]'
  },
  textClass: {
    type: String,
    default: 'text-white'
  }
});
</script>

<style scoped>
.card {
  max-width: 275px;
  max-height: 225px;
}
</style>
