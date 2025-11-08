<template>
  <div class="card">
    <h3>Áreas de Interés Profesional</h3>
    <p>Actualmente estoy enfocado y me interesa profundizar mis conocimientos en:</p>
    <ul class="lista-intereses">
      <li>Desarrollo Backend (especialmente con Java)</li>
      <li>Desarrollo Web Frontend (JavaScript y frameworks como Vue)</li>
      <li>Bases de Datos Relacionales (MySQL)</li>
      <li>Análisis de Datos y Scripting (Python)</li>
    </ul>
  </div>
</template>

<script setup>
</script>
<style scoped>

.card {
  background-color: #3a6ea5;
  color: white;
  
  padding: 25px;
  border-radius: 10px;
  margin-bottom: 25px;
  
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  text-align: left;
}

.lista-intereses {
  list-style-position: inside;
  text-align: left;
  margin-top: 15px;
  padding-left: 10px;
}

.lista-intereses li {
  margin-bottom: 8px;
}
</style>