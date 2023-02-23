<script setup lang="ts">
withDefaults(
  defineProps<{
    title?: string;
    color?: string;
  }>(),
  { title: "", color: "#000000" }
);
</script>

<template>
  <button :title="title || undefined">
    <slot />
  </button>
</template>

<style scoped>
button {
  color: #fff;
  background-color: v-bind("color");
  padding: 10px;
  border-radius: 10px;
  border: none;
}

button:hover {
  cursor: pointer;
  filter: opacity(0.8);
  outline: 2px solid v-bind("color");
  outline-offset: 2px;
}
</style>
