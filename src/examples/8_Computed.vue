<script setup lang="ts">
import { computed, ref } from "vue";

const num = ref(2);
const doubled = computed(() => num.value * 2);
</script>

<template>
  {{ doubled }}
</template>
