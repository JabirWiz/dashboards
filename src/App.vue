<script setup>
import { RouterView } from 'vue-router'
import Appbar from './components/Appbar.vue';
import Sidebar from './components/Sidebar.vue';
</script>

<template>
  <div class="d-flex">
    <RouterView />
    <!-- <Sidebar /> -->
    <!-- <Appbar /> -->
    <!-- <RouterView style="margin-top: 64px; margin-left: 256px; width: 100%; height: 100%;" /> -->
  </div>
</template>

<style scoped>
</style>
