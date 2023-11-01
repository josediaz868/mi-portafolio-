<template>
    <div class="proyecto">
      <h2>{{ proyecto.titulo }}</h2>
      <p>{{ proyecto.descripcion }}</p>
    </div>
  </template>
  
  <script>
  export default {
    props: ["proyecto"]
  };
  </script>
  
  <style scoped>
  /* Estilos específicos para el componente Proyecto */
  </style>
  