<template>
  <header class="header">
    <UpperContainer />

    <NavBar />
  </header>
</template>

<script setup>
import UpperContainer from './components/UpperContainer.vue';
import NavBar from './components/NavBar.vue';
</script>

<style scoped>
.header {
  background-color: white;
  font-family: 'Kanit', sans-serif;
  color: #EB4648;
  width: 100%;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  position: sticky;
  top: 0;
  z-index: 1000;
}
</style>
