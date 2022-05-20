<script setup lang="ts">
import { ref } from "vue";
import type { Note } from "@/types";
const notes = ref<Note[]>([{ title: "", body: "", createdAt: new Date() }]);
const createNote = () => {
  notes.value.push({
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
