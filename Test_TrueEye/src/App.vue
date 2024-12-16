<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import Header from './components/Header.vue'
</script>

<template>
    <div class="page-container">
      <Header />
      <RouterView />
    </div>

</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}

@import url('https://fonts.googleapis.com/css2?family=Kanit:wght@400;700&display=swap');

.layout {
  display: flex;
  height: 100%; /* Full viewport height */
  margin: 0;
}

.content {
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  width: 100%;
  overflow: auto;
}

.header {
  background-color: white;
  font-family: 'Kanit', sans-serif;
  color: #EB4648;
  width: 100%;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  position: sticky; /* Make the header stick to the top */
  top: 0;
  z-index: 1000; /* Ensure it appears above other content */
}
</style>