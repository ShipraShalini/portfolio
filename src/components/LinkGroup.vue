<script setup lang="ts">

import {defineProps} from "vue";
import {Link} from "../constants/links";

defineProps ({links: [] as () => Link[]})
</script>


<template>
  <div>
    <ul>
      <li v-for="link in links">
        <a :href="link.href">[{{ link.label }}]</a>
      </li>
    </ul>
  </div>

</template>


<style scoped>
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  font-size: 1em;
  float: left;
}

li a {
  display: block;
  color: white;
  text-align: center;
  padding: 16px;
  text-decoration: none;
}

li a:hover {
  color: rgb(59 130 246 / 0.5);
}
</style>