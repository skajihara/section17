<script setup lang="ts">
import { ref } from 'vue'

const count = ref<number | string>(0)
count.value = { id: '7', name: 'foo' }
</script>
<template>
  <h1>TypeScript</h1>
  <p>{{ count }}</p>
</template>
