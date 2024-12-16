<template>
  <header class="header">
    <div class="upper-container">
      <div class="logo-container">
        <h1 class="logo">TRUEEYE</h1>
        <p class="slogan">AI for life</p>
      </div>
      <div class="contact-container">
        <div class="contact-item">
          <span class="icon">📞</span>
          <p>080-227-3777</p>
        </div>
        <div class="divider"></div>
        <div class="contact-item">
          <span class="icon">📧</span>
          <p>info@trueeye.ai</p>
        </div>
      </div>
      <div class="buttons-container">
        <button class="contact-button">CONTACT</button>
        <button class="support-button">SUPPORT</button>
      </div>
    </div>
    <nav class="nav-bar">
      <ul class="menu">
        <li><a href="#">HOME</a></li>
        <li><a href="#">ABOUT US</a></li>
        <li><a href="#">SERVICE</a></li>
        <li><a href="#">NEWS & ACTIVITIES</a></li>
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
  </header>
</template>

<style scoped>
.header {
  background-color: white;
  font-family: 'Kanit', sans-serif;
  color: #EB4648;
  width: 100%;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  position: sticky; /* Make the header stick to the top */
  top: 0;
  z-index: 1000; /* Ensure it appears above other content */
}

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

.contact-container {
  display: flex;
  align-items: center;
  gap: 15px;
  font-size: 0.9rem;
}

.contact-item {
  display: flex;
  align-items: center;
  gap: 5px;
}

.divider {
  width: 1px;
  height: 20px;
  background-color: #ccc;
}

.icon {
  font-size: 1.2rem;
  color: #EB4648;
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
  position: relative;
  width: 20px;
  cursor: pointer;
}

@media (max-width: 768px) {
  .upper-container {
    flex-direction: column;
    text-align: center;
    gap: 15px;
  }

  .nav-bar {
    flex-direction: column;
    gap: 15px;
  }

  .menu {
    flex-direction: column;
    gap: 10px;
  }
}
</style>
