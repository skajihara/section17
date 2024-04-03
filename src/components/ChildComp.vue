<script setup lang="ts">
defineEmits<{
  update: [count: number]
  reset: [count: number]
}>()
</script>
<template>
  <h2>ChildComp</h2>
  <button @click="$emit('update', 100)">+100</button>
  <button @click="$emit('reset', 0)">reset</button>
</template>
