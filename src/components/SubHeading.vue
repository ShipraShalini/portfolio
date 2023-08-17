<script setup lang="ts">
import {defineProps} from "vue";

defineProps({ text: string })
</script>

<template>
  <h2>{{ text }}</h2>
</template>

<style scoped>
h2 {
  font-weight: 800;
}
</style>
