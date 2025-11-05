<template>
  <div class="projects-grid">
    <div class="card">
      <img src="../assets/java1.PNG" alt="Java Project 1" />
      <h3>Proyecto Integrador en Java - JuegoAhorjado en Consola</h3>
      <p>Este proyecto integrador, desarrollado en Java para consola, reinventa el clásico juego del "Ahorcado" con un
        enfoque educativo. El jugador se enfrenta a una serie de adivinanzas centradas en conceptos clave, palabras
        reservadas y fundamentos de la programación en Java.</p>

      <a href="https://github.com/HotCode2025/PI_SegundoSemestre-ByteNine" target="_blank" rel="noopener noreferrer"
        class="link">
        Ver proyecto
      </a>
    </div>

    <div class="card">
      <img src="../assets/java2.PNG" alt="Java Project 2" />
      <h3>Proyecto Integrador en Java - JuegoAhorajado en Interfaz Gráfica</h3>
      <p>Este proyecto integrador presenta una versión gráfica e interactiva del clásico juego "Ahorcado", desarrollada
        íntegramente en Java (Swing/JavaFX). El juego desafía al usuario con adivinanzas sobre conceptos, palabras clave
        y fundamentos de la programación en Java, todo presentado en una interfaz de usuario amigable e intuitiva.</p>

      <a href="https://github.com/HotCode2025/PI_SegundoSemestre-ByteNine" target="_blank" rel="noopener noreferrer"
        class="link">
        Ver proyecto
      </a>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
}

.card {
  background-color: #3a6ea5;
  color: white;
  padding: 25px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
}

.card img {
  width: 100%;
  border-radius: 8px;
  margin-bottom: 20px;
}

.card h3 {
  margin-bottom: 10px;
}

.card p {
  flex-grow: 1;
  margin-bottom: 20px;
}

.link {
  background-color: white;
  color: #3a6ea5;
  padding: 10px 20px;
  border-radius: 8px;
  text-decoration: none;
  font-weight: 600;
  text-align: center;
  transition: background-color 0.2s ease;
}

.link:hover {
  background-color: #f0f0f0;
}
</style>