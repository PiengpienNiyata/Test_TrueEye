<template>
    <div class="contact-item">
      <span class="icon">{{ icon }}</span>
      <p>{{ text }}</p>
    </div>
  </template>
  
  <script setup>
  defineProps({
    icon: String,
    text: String
  });
  </script>
  
  <style scoped>
  .contact-item {
    display: flex;
    align-items: center;
    gap: 5px;
  }
  
  .icon {
    font-size: 1.2rem;
    color: #EB4648;
  }
  </style>
  