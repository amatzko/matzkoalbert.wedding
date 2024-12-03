<template>
  <div class="contact-container">
    <NuxtLink to="/" class="back-arrow">←</NuxtLink>
    <h1 class="page-title">Contact Us</h1>
    
    <div class="contact-info">
      <div class="contact-person">
        <h2>Katie</h2>
        <p><strong>Phone:</strong> <a href="tel:+14404768738">(440) 476-8738</a></p>
        <p><strong>Email:</strong> <a href="mailto:kathleen@matzko.family">kathleen@matzko.family</a></p>
      </div>
      
      <div class="contact-person">
        <h2>Aidan</h2>
        <p><strong>Phone:</strong> <a href="tel:+15136004932">(513) 600-4932</a></p>
        <p><strong>Email:</strong> <a href="mailto:aidan@matzko.family">aidan@matzko.family</a></p>
      </div>
    </div>
    
    <div class="contact-message">
      <p>Feel free to reach out to us if you have any questions!</p>
    </div>
  </div>
</template>

<script setup lang="ts">
// No script needed for this component
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Satisfy&family=Old+Standard+TT&display=swap');

.contact-container {
  position: relative;
  max-width: 800px;
  margin: 0 auto;
  padding: 2rem;
  font-family: 'Old Standard TT', serif;
  color: #3a3a3a;
  background-color: #f9f3e6;
  border: 1px solid #d3c7a6;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.back-arrow {
  position: absolute;
  top: 1rem;
  left: 1rem;
  font-size: 1.5rem;
  color: #8b4513;
  text-decoration: none;
  transition: transform 0.2s ease;
}

.back-arrow:hover {
  transform: translateX(-3px);
}

.page-title {
  text-align: center;
  font-size: 3rem;
  color: #8b4513;
  margin-bottom: 2rem;
  font-family: 'Satisfy', cursive;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
}

.contact-info {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  margin-bottom: 2rem;
}

.contact-person {
  flex-basis: 45%;
  margin-bottom: 1rem;
}

h2 {
  font-size: 1.8rem;
  color: #8b4513;
  margin-bottom: 1rem;
  font-family: 'Playfair Display', serif;
  font-weight: 700;
}

p {
  line-height: 1.6;
  margin-bottom: 0.5rem;
  font-size: 1.1rem;
}

a {
  color: #3a3a3a;
  text-decoration: none;
  transition: color 0.3s ease;
}

a:hover {
  color: #8b4513;
}

.contact-message {
  text-align: center;
  margin-top: 2rem;
  font-style: italic;
}

@media (max-width: 768px) {
  .contact-container {
    padding: 1rem;
  }

  .page-title {
    font-size: 2.5rem;
  }

  .contact-person {
    flex-basis: 100%;
  }

  h2 {
    font-size: 1.5rem;
  }

  p {
    font-size: 1rem;
  }
}
</style>
