<script setup lang="ts">
import SideBarButton from './SideBarButton.vue'
</script>

<template>
  <div :class="$style.container">
    <SideBarButton title="Apple" />
    <SideBarButton title="Banana" />
    <SideBarButton title="Orange" />
    <SideBarButton title="Lemon" />
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
