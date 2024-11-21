<template>
  <div class="registry-container">
    <h1 class="page-title">Wedding Registry</h1>

    <div class="welcome-message">
      <p>
        Don't feel obligated to gift us anything! We've made a wonderful home for ourselves the last few years (and some of you have already gifted us) &#128522; but if you still want to...
      </p>
    </div>
    
    <div class="registry-section">
      <h2>Amazon Registry</h2>
      <p>Here's a few fun things:</p>
      <a href="your-amazon-registry-link-here" target="_blank" rel="noopener noreferrer" class="registry-button">
        View Amazon Registry
      </a>
    </div>

    <div class="digital-gifts">
      <h2>Digital Gifts</h2>
      <p>Or if you want to contribute to our honeymoon/house/future dog fund:</p>
      <div class="payment-options">
        <a href="your-venmo-link-here" target="_blank" rel="noopener noreferrer" class="payment-button venmo">
          Venmo
        </a>
        <a href="your-paypal-link-here" target="_blank" rel="noopener noreferrer" class="payment-button paypal">
          PayPal
        </a>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// No script needed for this update
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Satisfy&family=Old+Standard+TT&display=swap');
.welcome-message {
  margin-bottom: 2rem;
  text-align: center;
  padding: 1.5rem;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.welcome-message p {
  max-width: 600px;
  margin: 0 auto;
  line-height: 1.8;
}
.registry-container {
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

.page-title {
  text-align: center;
  font-size: 3rem;
  color: #8b4513;
  margin-bottom: 2rem;
  font-family: 'Satisfy', cursive;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
}

h2 {
  font-size: 2rem;
  color: #8b4513;
  margin-bottom: 1rem;
  text-align: center;
  font-family: 'Playfair Display', serif;
  font-weight: 700;
}

.registry-section, .digital-gifts {
  margin-bottom: 2rem;
  text-align: center;
  padding: 1.5rem;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

p {
  line-height: 1.6;
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.registry-button, .payment-button {
  display: inline-block;
  background-color: #8b4513;
  color: #f9f3e6;
  border: none;
  padding: 12px 24px;
  font-size: 1.1rem;
  cursor: pointer;
  border-radius: 5px;
  transition: background-color 0.3s ease;
  font-family: 'Playfair Display', serif;
  text-decoration: none;
  margin: 1rem 0;
}

.registry-button:hover, .payment-button:hover {
  background-color: #a0522d;
}

.payment-options {
  display: flex;
  justify-content: center;
  gap: 2rem;
  margin-top: 1rem;
}

@media (max-width: 768px) {
  .registry-container {
    padding: 1rem;
  }

  .page-title {
    font-size: 2.5rem;
  }

  h2 {
    font-size: 1.8rem;
  }

  p {
    font-size: 1rem;
  }

  .payment-options {
    flex-direction: column;
    align-items: center;
    gap: 1rem;
  }

  .payment-button {
    width: 80%;
  }
}
</style>