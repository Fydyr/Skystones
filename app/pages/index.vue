<template>
  <div>
    <HeroComponent />
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  layout: 'default'
})

useHead({
  title: 'Home - Aeroliths',
  meta: [
    { name: 'description', content: 'Welcome to Aeroliths, a fan-made game inspired by Skystones from the Skylanders franchise' }
  ]
})
</script>