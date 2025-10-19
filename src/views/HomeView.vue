<script setup>
import homePage from '../components/HomePage.vue';
</script>

<template>
  <main>
    <nav class="main_nav">
      <router-link to="/">Muro</router-link>
      <router-link to="/about">Info</router-link>
      <router-link to="/photos">Fotos</router-link>
    </nav>
    <homePage />
  </main>
</template>

<style>
main {
  display: flex;
  position: relative;
  min-height: 100vh;
  margin-top: 150px;
}

/* @media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
} */
</style>
