<script setup lang="ts">
defineProps<{
  title: string
}>()
</script>
<template>
  <div :class="$style.container">
    <div :class="$style.buttontext">{{ title }}</div>
  </div>
</template>
<style module>
.container {
  width: 100%;
  height: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.buttontext {
  align-self: center;
  text-align: center;
}
</style>
