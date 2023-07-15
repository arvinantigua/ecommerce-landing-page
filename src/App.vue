<script setup>
  import { RouterLink, RouterView } from 'vue-router'
  import Navbar from './components/Navigation.vue'
</script>

<template>
  <div class="container-fluid px-0">
    <Navbar />
    <RouterView />
  </div>
</template>
