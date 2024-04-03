<script setup lang="ts">
import { ref } from 'vue'
import ChildComp from './components/ChildComp.vue'
const userInput = ref('')
</script>
<template>
  <h1>TypeScript</h1>
  <ChildComp v-model="userInput" />
  <p>userInput:{{ userInput }}</p>
</template>
