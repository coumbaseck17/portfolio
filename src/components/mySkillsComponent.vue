<script setup>
const props = defineProps(['title', 'description']);

</script>

<template>
  <div class="bg-white p-4 mb-4 hover:-translate-y-3 hover:border-2 hover:border-fuchsia-200 hover:bg-fuchsia-100 transition-all duration-500">
    <h2 class="text-xl mb-2">{{ title }}</h2>
    <p class="text-balance">{{ description }}</p>
    </div>
</template>

<style scoped>
/* Add your component-specific styles here */
</style>
