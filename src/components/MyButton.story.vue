<script setup lang="ts">
import MyButton from "./MyButton.vue";
</script>

<template>
  <Story>
    <Variant title="Default">
      <MyButton>Default</MyButton>
    </Variant>
    <Variant title="Success">
      <MyButton color="#4caf50">Success</MyButton>
    </Variant>
    <Variant title="Error">
      <MyButton color="#f44336">Error</MyButton>
    </Variant>
    <Variant title="Info">
      <MyButton color="#2196f3">Info</MyButton>
    </Variant>
  </Story>
</template>
