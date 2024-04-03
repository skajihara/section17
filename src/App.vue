<script setup lang="ts">
import ChildComp from './components/ChildComp.vue'
</script>
<template>
  <h1>TypeScript</h1>
  <ChildComp :name="'A'" :level="10" />
</template>
