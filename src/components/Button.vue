<script setup lang="ts">
// import { ref } from 'vue'

defineProps<{ description: string, active? : boolean , color?: 'off' }>()

const cor = {
  1 : "off",
  2 : "error",
  3 : "warn",
  4 : "info",
  5 : "debug",
  6 : "trace",
  7 : "reset"
}

</script>

<template>
  <button>{{ description }}</button>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}

button {
  cursor: pointer;
  user-select: none;
}
</style>
