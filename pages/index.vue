<template>
  <div class="home-container">
    
    <h1 class="wedding-title">Katie & Aidan's Wedding</h1>
    <div class="location-image">
        <img src="/images/park-of-roses.jpg" alt="Columbus Park of Roses" />
    </div>
    <div class="welcome-message">
      <p>
        After eloping in April of 2024, we are thrilled to celebrate our love again with all of you!
      </p>
    </div>   
   
    <div class="wedding-date">
      <h2>When?</h2>
      <p>April 26, 2025</p>
      <p>Arrival is at 11:30AM. The ceremony begins at 12:00 PM and will be followed by a lunch reception (with a bar). The reception will end around 3:45 PM.</p>
    </div>

    <div class="location-details">
      <h2>Where?</h2>
      <address>
        <a href="https://maps.app.goo.gl/UP5ebr73kkykoTmHA" target="_blank" rel="noopener noreferrer">
          Whetstone Shelterhouse<br>
          3901 N. High St<br>
          Columbus, OH 43214<br>
        </a>
      </address>
    </div>

    <div class="dress-code">
      <h2>What should I wear?</h2>
      <p>
        Festive or cocktail attire (dresses, dress shirt & pants, etc.) would be great! There is no official theme. The ceremony will be outdoors if weather permits, so dress accordingly.
      </p>
    </div>

    <div class="afters">
      <h2>What are we doing later?</h2>
      <p>
        We are attending <a href="https://landgrantbrewing.com/" target="_blank" rel="noopener noreferrer">Land Grant Brewing</a> for drinks after the wedding! We have a tent reserved from 6:30PM to close.
      </p>
    </div>

    <div class="accommodations">
      <h2>Travelling from out of town?</h2>
      <p>
        The Columbus airport (CMH) is located only 15 minutes from downtown. We will not have a hotel room block, but we recommend the following hotels:
      </p>
      <ul>
        <li><a href="https://www.marriott.com/en-us/hotels/cmhdm-le-meridien-columbus-the-joseph/overview/" target="_blank" rel="noopener noreferrer">La Meridien (~$350/night)</a></li>
        <li><a href="https://www.hilton.com/en/hotels/cmhdwhh-hilton-columbus-downtown/" target="_blank" rel="noopener noreferrer">Hiltown Columbus Downtown (~$240/night)</a></li>
        <li><a href="https://www.marriott.com/en-us/hotels/cmhcy-courtyard-columbus-downtown/overview/" target="_blank" rel="noopener noreferrer">Courtyard Downtown Columbus (~$125/night)</a></li>
      </ul>
      <p>
        We have also had good experiences with Airbnb's in the area.
      </p>
    </div>

    <div class="rsvp-section">
      <h2>RSVP</h2>
      <p>Please let us know if you can attend by February 16th, 2025.</p>
      <div class="button-row">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSfJfL5um3uuaZvPM5kT37MbTvgW554D6GEurbYfpNRknsknDg/viewform?usp=sf_link" target="_blank" rel="noopener noreferrer" class="rsvp-button">
          RSVP
        </a>
        <NuxtLink to="/contact" class="rsvp-button">
          Contact Us
        </NuxtLink>
        <NuxtLink to="/registry" class="rsvp-button">
          Registry
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// No script needed for this update
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Satisfy&family=Old+Standard+TT&display=swap');

.home-container {
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

.wedding-title {
  text-align: center;
  font-size: 3.5rem;
  color: #8b4513;
  margin-bottom: 2rem;
  font-family: 'Satisfy', cursive;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.1);
}

.button-row {
  display: flex;
  justify-content: center;
  gap: 1rem;
  flex-wrap: wrap;
  margin-top: 1.5rem;
}


h2 {
  font-size: 2rem;
  color: #8b4513;
  margin-bottom: 1rem;
  text-align: center;
  font-family: 'Playfair Display', serif;
  font-weight: 700;
}

.wedding-date, .location-details, .welcome-message, .rsvp-section {
  margin-bottom: 2rem;
  text-align: center;
}

.wedding-date p {
  font-size: 1.5rem;
  font-weight: bold;
  font-family: 'Playfair Display', serif;
}

address {
  font-style: normal;
  line-height: 1.6;
  margin-bottom: 1rem;
}

p {
  line-height: 1.6;
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.rsvp-button {
  display: inline-block;
  background-color: #8b4513;
  color: #f9f3e6;
  border: none;
  padding: 10px 20px;
  font-size: 1.1rem;
  cursor: pointer;
  border-radius: 5px;
  transition: background-color 0.3s ease;
  font-family: 'Playfair Display', serif;
  text-decoration: none;
}

.rsvp-button:hover {
  background-color: #a0522d;
}

@media (max-width: 768px) {
  .home-container {
    padding: 1rem;
  }

  .wedding-title {
    font-size: 2.5rem;
  }

  h2 {
    font-size: 1.8rem;
  }

  p, address {
    font-size: 1rem;
  }
}

.location-image {
  margin-top: 1rem;
  text-align: center;
}

.location-image img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

address a {
  color: #3a3a3a;
  text-decoration: none;
  transition: color 0.3s ease;
}

address a:hover {
  color: #8b4513;
}
</style>
