<template>
    <div class="upper-container">
      <!-- Logo -->
      <div class="logo-container">
        <h1 class="logo">TRUEEYE</h1>
        <p class="slogan">AI for life</p>
      </div>
  
      <!-- Contact Info -->
      <div class="contact-container">
        <ContactItem icon="📞" text="080-227-3777" />
        <div class="divider"></div>
        <ContactItem icon="📧" text="info@trueeye.ai" />
      </div>
  
      <!-- Buttons -->
      <div class="buttons-container">
        <button class="contact-button">CONTACT</button>
        <button class="support-button">SUPPORT</button>
      </div>
    </div>
  </template>
  
  <script setup>
  import ContactItem from './ContactItem.vue';
  </script>
  
  <style scoped>
  .upper-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 30px;
    box-shadow: 0 1px 2.5px rgba(0, 0, 0, 0.2);
  }
  
  .logo-container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  
  .logo {
    font-size: 2rem;
    font-weight: bold;
    margin: 0;
  }
  
  .slogan {
    font-size: 0.9rem;
    color: gray;
    margin: 0;
  }
  
  .divider {
    width: 1px;
    height: 20px;
    background-color: #ccc;
  }
  
  .buttons-container {
    display: flex;
    gap: 15px;
  }
  
  .contact-button,
  .support-button {
    min-width: 120px;
    background-color: #EB4648;
    color: white;
    border: none;
    padding: 8px 16px;
    font-size: 0.9rem;
    cursor: pointer;
    border-radius: 25px;
    text-transform: uppercase;
  }
  
  .contact-button:hover,
  .support-button:hover {
    background-color: #c0392b;
  }
  </style>
  