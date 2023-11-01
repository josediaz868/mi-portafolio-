<template>
    <div id="app">
      <header>
        <h1>Bienvenido a mi portafolio</h1>
      </header>
      <main>
        <Proyecto
          v-for="proyecto in proyectos"
          :key="proyecto.id"
          :proyecto="proyecto"
        ></Proyecto>
      </main>
    </div>
  </template>
  
  <script>
  import Proyecto from "./components/Proyecto.vue";
  
  export default {
    name: "App",
    components: {
      Proyecto
    },
    data() {
      return {
        proyectos: [
          { id: 1, titulo: "Proyecto 1", descripcion: "Descripción del proyecto 1" },
          { id: 2, titulo: "Proyecto 2", descripcion: "Descripción del proyecto 2" },
          // ... más proyectos
        ]
      };
    }
  };
  </script>
  
  <style>
  /* Estilos globales para tu aplicación */
  </style>
  