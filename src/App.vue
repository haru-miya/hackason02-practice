<script setup lang="ts">
import { ref } from 'vue'
import MainContent from './components/MainContent.vue'
import SideBar from './components/SideBar.vue'
const fruit = ref('')
</script>

<template>
  <main :class="$style.container">
    <SideBar v-model:fruit="fruit" />
    <MainContent :title="fruit" />
  </main>
</template>

<style module>
.container {
  height: 100vh;
  display: flex;
  flex-direction: row;
}
</style>
