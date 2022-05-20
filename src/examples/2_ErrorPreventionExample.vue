<!-- <script setup lang="ts"> -->
<script setup>
import { ref } from "vue";
const notes = ref([{ title: "", body: "", createdAt: new Date() }]);
const createNote = () => {
  notes.value.push({
    title: "My new note",
    body: "hello world",
    createdAt: Date.now(),
  });
};
</script>

<template>
  {{ notes }}
  <button @click="createNote">Create Note</button>
</template>
