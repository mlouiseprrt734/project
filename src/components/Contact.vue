<script setup>
const handleSubmit = (event) => {
  event.preventDefault()
  // Add form submission logic here
}
</script>

<template>
  <section id="contact" class="contact">
    <h2>Get In Touch</h2>
    <div class="contact-container">
      <form @submit="handleSubmit" class="contact-form">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" required>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" rows="5" required></textarea>
        </div>
        <button type="submit" class="submit-button">Send Message</button>
      </form>
    </div>
  </section>
</template>

<style scoped>
.contact {
  padding: 5rem 2rem;
  background-color: white;
}

h2 {
  text-align: center;
  margin-bottom: 3rem;
  color: #2c3e50;
}

.contact-container {
  max-width: 600px;
  margin: 0 auto;
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

label {
  color: #2c3e50;
  font-weight: 500;
}

input, textarea {
  padding: 0.8rem;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 1rem;
}

.submit-button {
  background-color: #3498db;
  color: white;
  padding: 1rem;
  border: none;
  border-radius: 5px;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.submit-button:hover {
  background-color: #2980b9;
}
</style>