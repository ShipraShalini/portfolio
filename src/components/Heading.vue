<script setup lang="ts">
defineProps<{ text: string }>()
</script>

<template>
  <h1>{{ text }}</h1>
</template>

<style scoped>
h1 {
  font-weight: 800;
}
</style>
