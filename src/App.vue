<script setup lang="ts">
import Header from '@/components/Header.vue';
import Home from './views/Home.vue';
</script>

<template>
  <header>
    <Header />
  </header>

  <Home />
</template>

<style scoped>
  header {
    position: relative;

    max-height: 100vh;
    line-height: 1.5;
  }

</style>
