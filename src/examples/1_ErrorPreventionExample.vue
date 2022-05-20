<script setup lang="ts">
import { ref } from "vue";
const notes = ref([{ title: "", body: "", createdAt: new Date() }]);
const createNote = () => {
  // eslint-disable-next-line vue/no-ref-as-operand
  notes.push({
    title: "My new note",
    body: "hello world",
    createdAt: new Date(),
  });
};
</script>

<template>
  {{ notes }}
  <button @click="createNote">Create Note</button>
</template>
