<script setup lang="ts">
defineProps<{
  color: string
}>()
</script>

<template>
  <div :class="$style.container"></div>
</template>

<style module>
.container {
  width: 200px;
  height: 200px;
  background-color: v-bind(color);
  border-radius: 10px;
}
</style>
