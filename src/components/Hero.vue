<script setup>
</script>

<template>
  <section class="hero">
    <div class="hero-content">
      <h1>Transforming Businesses Through AI Integration</h1>
      <p>Empowering companies with cutting-edge AI solutions and expert training</p>
      <button class="cta-button" @click="$emit('scrollToServices')">
        Explore Our Services
      </button>
    </div>
  </section>
</template>

<style scoped>
.hero {
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, #3498db, #2c3e50);
  color: white;
  text-align: center;
  padding: 0 2rem;
}

.hero-content {
  max-width: 800px;
}

h1 {
  font-size: 3.5rem;
  margin-bottom: 1.5rem;
}

p {
  font-size: 1.5rem;
  margin-bottom: 2rem;
  opacity: 0.9;
}

.cta-button {
  padding: 1rem 2rem;
  font-size: 1.2rem;
  background-color: #e74c3c;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #c0392b;
}
</style>