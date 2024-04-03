<script setup lang="ts">
import { ref } from 'vue'
import ChildComp from './components/ChildComp.vue'
const count = ref(0)
function onClick(value) {
  count.value += value
}
function onReset(value) {
  count.value = 0
}
</script>
<template>
  <h1>TypeScript</h1>
  <button @click="count++">+1</button>
  <ChildComp @update="onClick" @reset="onReset" />
  <p>{{ count }}</p>
</template>
