<script setup>
const services = [
  {
    title: 'AI Integration',
    description: 'Custom AI solutions tailored to your business needs. We help companies implement and optimize AI technologies.',
    icon: '🤖'
  },
  {
    title: 'Training & Education',
    description: 'Comprehensive AI training programs for teams and organizations. Learn how to leverage AI effectively.',
    icon: '📚'
  },
  {
    title: 'Consulting',
    description: 'Strategic guidance on AI implementation and digital transformation for your business.',
    icon: '💡'
  }
]
</script>

<template>
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="services-grid">
      <div v-for="service in services" :key="service.title" class="service-card">
        <div class="service-icon">{{ service.icon }}</div>
        <h3>{{ service.title }}</h3>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
.services {
  padding: 5rem 2rem;
  background-color: #f8f9fa;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
  color: #2c3e50;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

.service-card {
  background: white;
  padding: 2rem;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  transition: transform 0.3s ease;
}

.service-card:hover {
  transform: translateY(-5px);
}

.service-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

h3 {
  color: #3498db;
  margin-bottom: 1rem;
}

p {
  color: #666;
  line-height: 1.6;
}
</style>