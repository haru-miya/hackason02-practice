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
.container:hover {
  background-color: rgb(200, 200, 200);
  cursor: pointer;
}
.buttontext {
  align-self: center;
  text-align: center;
}
</style>
