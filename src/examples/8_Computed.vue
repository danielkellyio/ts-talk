<script setup lang="ts">
import { computed, ref } from "vue";

const genrePreference = ref("comedy");
const movieSuggestion = computed((): string => {
  const pref = genrePreference.value;
  const movieMap = {
    comedy: "Bill and Ted's Excellend Adventure",
    drama: "Jurassic Park",
    romance: "Elizabeth Town",
  };
  return Object.keys(movieMap).includes(pref) ? movieMap[pref] : "Marvel Movie";
});
</script>

<template>
  {{ movieSuggestion }}
</template>
