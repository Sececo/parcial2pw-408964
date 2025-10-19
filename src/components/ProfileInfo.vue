<script setup>
import { defineProps } from 'vue';

// 1. Define las props que el componente espera recibir
const props = defineProps({
  userName: {
    type: String,
    default: 'Nombre', // Valor por defecto si no se pasa nada
  }
});

</script>

<template>
  <img
      src="../assets/Xbox perfil.jpg"
      alt="Foto de perfil"
      class="foto_perfil"
    />

  <h2 class="subrayado">{{ props.userName }}</h2>
  <h3>Información</h3>
</template>