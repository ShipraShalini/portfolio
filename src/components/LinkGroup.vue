<script setup lang="ts">

interface Link {
  label: string
  href: string
}
const Links: Link[] = [
  {label: "github", href: "https://github.com/shiprashalini/"},
  {label: "linkedin", href: "https://github.com/shiprashalini"},
  {label: "source code", href: "https://github.com/shiprashalini/portfolio-we"},
  {label: "infra code", href: "https://github.com/shiprashalini/portfolio-infra"},
]
</script>


<template>
  <div>
    <ul>
      <li v-for="link in Links">
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