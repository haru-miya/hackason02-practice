<script setup lang="ts">
defineProps<{
  title: string
}>()
const msg = (a: string) => {
  return `${a} `.repeat(30).trim()
}
</script>

<template>
  <div :class="$style.container">
    <h1>Title</h1>
    <p>{{ msg(title) }}</p>
  </div>
</template>

<style module>
.container {
  width: 1000px;
  height: 100vh;
  border: 1px dotted red;
  margin: auto;
  padding-top: 120px;
}
</style>
