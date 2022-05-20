<script setup lang="ts">
defineProps<{
  count: number;
}>();
defineEmits(["increment"]);
</script>
