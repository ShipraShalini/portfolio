<script setup lang="ts">
import {defineProps} from "vue";
defineProps({ text: String })
</script>

<template>
  <h1>{{ text }}</h1>
</template>

<style scoped>
h1 {
  font-weight: 800;
}
</style>
