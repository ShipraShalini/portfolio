<script setup lang="ts">
import {defineProps} from "vue";
defineProps({ link: string })
</script>

<template>
  <div class="footer">
    <span>Inspired by </span><span><a :href="link">[{{ link }}]</a></span>
  </div>
</template>

<style scoped>
.footer{
 position:fixed;
 bottom:0;
  text-align: center;
}
.footer a {
  color: white;
}
</style>
