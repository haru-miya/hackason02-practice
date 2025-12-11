<script setup lang="ts">
import SideBarButton from './SideBarButton.vue'
const fruit = defineModel<string>('fruit')
</script>

<template>
  <div :class="$style.container">
    <SideBarButton title="Apple" @click="fruit = 'Apple'" />
    <SideBarButton title="Banana" @click="fruit = 'Banana'" />
    <SideBarButton title="Orange" @click="fruit = 'Orange'" />
    <SideBarButton title="Lemon" @click="fruit = 'Lemon'" />
  </div>
</template>

<style module>
.container {
  width: 200px;
  height: 100vh;
  background-color: rgb(227, 225, 225);
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
