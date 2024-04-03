<script setup lang="ts">
import { computed, ref } from 'vue'

const count = ref(0)
const doubleCount = computed(() => {
  if (count.value > 3) return 100
  return count.value * 2
})
doubleCount.value
function countUp(event: MouseEvent) {
  count.value++
  console.log(event.clientX)
}
</script>
<template>
  <h1>TypeScript</h1>
  <button @click="countUp">+1</button>
  <p>count: {{ count }}</p>
</template>
