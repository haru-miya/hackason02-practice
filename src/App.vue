<script setup lang="ts">
import MainContent from './components/MainContent.vue'
import SideBar from './components/SideBar.vue'
</script>

<template>
  <main class="container">
    <SideBar />
    <MainContent />
  </main>
</template>

<style scoped>
.container {
  height: 100vh;
  display: flex;
  flex-direction: row;
}
</style>
