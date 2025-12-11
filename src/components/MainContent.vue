<script setup lang="ts">
import MainContenBox from './MainContenBox.vue'

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
    <div :class="$style.contentBox">
      <MainContenBox color="red" />
      <MainContenBox color="lime" />
      <MainContenBox color="blue" />
    </div>
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
.contentBox {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-top: 40px;
}
</style>
