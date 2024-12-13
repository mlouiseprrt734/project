<script setup>
import Hero from './components/Hero.vue'
import Services from './components/Services.vue'
import Contact from './components/Contact.vue'
</script>

<template>
  <div class="app-container">
    <nav class="navbar">
      <div class="logo">AI Solutions</div>
      <div class="nav-links">
        <a href="#services">Services</a>
        <a href="#contact">Contact</a>
      </div>
    </nav>
    
    <Hero />
    <Services />
    <Contact />
  </div>
</template>

<style>
.app-container {
  min-height: 100vh;
  background-color: #ffffff;
  color: #2c3e50;
}

.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.5rem 2rem;
  background-color: rgba(255, 255, 255, 0.95);
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  z-index: 1000;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  color: #3498db;
}

.nav-links {
  display: flex;
  gap: 2rem;
}

.nav-links a {
  color: #2c3e50;
  text-decoration: none;
  font-weight: 500;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #3498db;
}
</style>