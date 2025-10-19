<script setup>
import photosPage from '../components/PhotosPage.vue';
</script>

<template>
  <main>
    <nav class="main_nav">
      <router-link to="/">Muro</router-link>
      <router-link to="/about">Info</router-link>
      <router-link to="/photos">Fotos</router-link>
    </nav>
    <photosPage />
  </main>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>