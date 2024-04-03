<script setup lang="ts">
const [model, modifiers] = defineModel<string, 'trim' | 'uppercase'>({ required: true })
modifiers.uppercase
</script>
<template>
  <h2>ChildComp</h2>
  <input v-model="model" type="text" />
  <p>model:{{ model }}</p>
</template>
