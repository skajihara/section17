<script setup lang="ts">
interface Course {
  name?: string
  level?: number
}
const props = withDefaults(defineProps<Course>(), {
  name: 'default course',
  level: 0
})
</script>
<template>
  <h2>ChildComp</h2>
  <p>course name : {{ name }}</p>
  <p>course level : {{ level }}</p>
</template>
