<script setup lang="ts">
import { reactive } from "vue";
// interface Site {
//   name: string;
//   url: string;
//   courses: string[];
// }
const site = reactive({
  name: "Vue School",
  url: "https://vueschool.io",
  courses: [
    "TypeScript Fundamentals",
    "TypeScript with Vue.js 3",
    "Pinia: The Enjoyable Vue Store",
    "Rapid Testing with Vitest",
    "Nuxt.js 3 Fundamentals",
  ],
});
</script>

<template>
  {{ site }}
</template>
