<script setup lang="ts">
import { ref } from "vue";
import type { Note } from "@/types";
const notes = ref<Note[]>([{ title: "", text: "", createdAt: new Date() }]);
const createNote = () => {
  notes.value.push({
    title: "My new note",
    text: "hello world",
    createdAt: new Date(),
  });
};
</script>

<template>
  {{ notes.map((n) => n.title).join(",") }}
  <button @click="createNote">Create Note</button>
</template>
