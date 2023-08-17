<script setup lang="ts">
import LinkGroup from "./components/LinkGroup.vue";
import Heading from "./components/Heading.vue";
import SubHeading from "./components/SubHeading.vue";
import Footer from "./components/Footer.vue";
import {links} from "./constants/links";
</script>

<template>

  <Heading text="Shipra Shalini" />
  <SubHeading text="Python & DevOps Engineer"/>
  <LinkGroup :links="links" />
  <Footer link="https://lawzava.com" />
</template>

<style scoped>
</style>
