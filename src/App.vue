<script setup>
import Card from './components/Cards.vue'
import Menubar from './components/MenuBar.vue'

</script>

<template>

  <header>
      
  </header>

  <Menubar />

  <main class="card-container">
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
      <Card />
  </main>
</template>

<style scoped>
.card-container {
    position: relative;
    top: 2rem;
    display: flex;
    gap: 20px; /* Add some space between the cards */
    justify-content: start; /* Align cards to the left, or use center for centering */
    flex-wrap: wrap; /* Ensure wrapping if the screen is small */
}
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
