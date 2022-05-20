<script setup lang="ts">
import { reactive } from "vue";
// interface VueEvent {
//   name: string;
//   location: string;
//   organizers: string[];
// }
const conference = reactive({
  name: "Vue.js Global Summit",
  location: "online",
  organizers: [
    "Madina Alyakbarova",
    "Ed Nedin",
    "Nik Petrov",
    "Pavlo Pankratov",
  ],
});
</script>

<template>
  {{ conference }}
</template>
