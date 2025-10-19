<script setup>
import { ref } from 'vue';
// importar el componente hijo
import ProfileInfo from './ProfileInfo.vue'; // 1. Importa el componente Hijo

const name = ref('Nombre'); // Inicializa 'name' con un valor por defecto para mostrar 'Nombre' al inicio
</script>

<template>
  <section class="main_section_perfil"
    id="main_section_perfil_id">
    <input
      type="text"
      v-model="name"
      placeholder="Tu nombre"
      class="input_nombre_perfil">
<!-- usar eel hijo desde el padre -->
    <ProfileInfo :userName="name" /> 
    <h3 class="subrayado"><span>X</span> Amigos</h3>
    <div class="main_section_div_amigos">
      <a clas="amigo"
        ><img src="../assets/Xbox perfil.jpg" class="amigo" alt="perfil_amigo"
      /></a>
      </div>
    <div class="info_img_dos">
      <p>Ver Todos</p>
    </div>
  </section>
  <section class="main_section_muro" id="muro">
        <div class="crear_publicacion">
          <input
            type="text"
            placeholder="Escribe algo..."
            class="input_publicacion"
          />
          <br />
          <input type="file" id="subir_archivo" class="boton_subir_archivo" />
          <button type="submit">Compartir</button>
          <!-- ventana compartir -->
        </div>
        <div class="muro_publicaciones">
          <div>
            <h2>Nombre</h2>
            <img class="amigo" src="../assets/Xbox perfil.jpg" alt="" />
          </div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
          <div class="info_social">
            <button>👍Like</button>
            <button>🔗compartir</button>
          </div>
        </div>
      </section>
</template>
