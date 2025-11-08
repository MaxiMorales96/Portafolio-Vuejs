<template>
  <div class="card">
    <h3>Lenguajes en proceso de aprendizaje en programación</h3>
    <p>Estas son algunas de las tecnologías en las que tengo conocimientos:</p>
    <ul class="lista-habilidades">
      <li>Java</li>
      <li>JavaScript</li>
      <li>Python</li>
      <li>MySQL</li>
      <li>Vue.js</li>
      <li>HTML & CSS</li>
    </ul>
  </div>
</template>

<script setup></script>
<style scoped>
.card {
  background-color: #f9fbfd;
  color: #333;
  padding: 25px;
  border-radius: 10px;
  margin-bottom: 25px;
  box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
  border: 2px dashed #3a6ea5;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
  text-align: left;
}

.lista-habilidades {
  list-style-type: none;
  padding: 0;
  margin-top: 15px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 10px;
}

.lista-habilidades li {
  background-color: #3a6ea5;
  color: white;
  padding: 8px 15px;
  border-radius: 20px;
  font-weight: 500;
}
</style>