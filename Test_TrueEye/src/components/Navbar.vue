<template>
    <nav class="nav-bar">
      <ul class="menu">
        <li v-for="item in menuItems" :key="item">
          <a href="#">{{ item }}</a>
        </li>
      </ul>
  
      <div class="extras">
        <div class="social-media">
          <a href="#">Facebook</a>
          <a href="#">LINE</a>
        </div>
  
        <div class="language-change">
          <a href="#" class="lang-icon">🇹🇭</a>
          <input type="checkbox" class="check" />
          <a href="#" class="lang-icon">🇬🇧</a>
        </div>
      </div>
    </nav>
  </template>
  
  <script setup>
  const menuItems = ['HOME', 'ABOUT US', 'SERVICE', 'NEWS & ACTIVITIES'];
  </script>
  
  <style scoped>
  .nav-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 30px;
    border-top: 1px solid #f0f0f0;
  }
  
  .menu {
    list-style: none;
    display: flex;
    gap: 25px;
    padding: 0;
    margin: 0;
  }
  
  .menu a {
    text-decoration: none;
    color: #EB4648;
    font-weight: bold;
  }
  
  .menu a:hover {
    text-decoration: underline;
  }
  
  .extras {
    display: flex;
    align-items: center;
    gap: 20px;
  }
  
  .social-media {
    display: flex;
    gap: 15px;
  }
  
  .social-media a {
    text-decoration: none;
    font-size: 0.9rem;
    color: gray;
  }
  
  .social-media a:hover {
    color: #EB4648;
  }
  
  .language-change {
    display: flex;
    align-items: center;
    gap: 5px;
  }
  
  .lang-icon {
    font-size: 1.2rem;
    cursor: pointer;
  }
  
  .check {
    width: 20px;
    cursor: pointer;
  }
  </style>
  