<script setup lang="ts">
import SideBarButton from './SideBarButton.vue'
</script>

<template>
  <div :class="$style.container">
    <SideBarButton />
    <SideBarButton />
    <SideBarButton />
    <SideBarButton />
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
