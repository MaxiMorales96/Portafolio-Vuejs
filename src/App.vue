<template>
  <div>
    <header>
      <h2>Futuro Programador</h2>
      <nav>
        <a href="#">Inicio</a>
        <a href="#contacto">Contacto</a>
        <a href="#experiencia">Experiencia</a>
        <a href="#proyectos">Proyectos</a>
      </nav>
    </header>

    <section class="hero">
      <div class="hero-text">
        <p>¡Bienvenidos a mi Portafolio Vue!</p>
        <h1>Maximiliano A Morales</h1>
        <p>Actualmente estudio Programación en la UTN, impulsado por mi interés en la tecnología. Además de mi
          formación, cuento con experiencia práctica en la reparación de celulares.</p>
        <button>+54 9 2984661349</button>
        <div class="socials">
          <a href="https://www.linkedin.com/in/maxi-morales-9b4541393/" target="_blank"><img src="./assets/linkedin.svg"
              alt="LinkedIn" /></a>
          <a href="https://github.com/MaxiMorales96" target="_blank"><img src="./assets/github.svg" alt="GitHub" /></a>
          <a href="https://www.instagram.com/m.a.mor712/" target="_blank"><img src="./assets/instagram.svg"
              alt="Instagram" /></a>
        </div>
      </div>
      <img src="./assets/photo.jpg" alt="Foto de Maximiliano A Morales" />
    </section>

    <section id="experiencia">
      <ExperienciaComponente />
    </section>

    <section id="proyectos" class="proyectos">
      <div class="linea-decorativa">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
      </div>
      <h2>Proyectos</h2>
      <ProyectosComponente />
    </section>
    <footer style="text-align:center;padding:30px 0;color:#6b7a86">© 2025 Maximiliano A Morales - Portafolio web - UTN FRSR</footer>
  </div>
</template>

<style>
nav a {
  background-color: #3a6ea5;
  color: white;
  border: none;
  border-radius: 10px;
  padding: 12px 25px;
  font-size: 1em;
  cursor: pointer;
  text-decoration: none;
  margin: 0 5px;
  transition: background-color 0.2s ease-in-out;
}

header nav a:hover {
  background-color: #345b8f;
}
</style>

<script setup>
import ProyectosComponente from './components/ProyectosComponente.vue'
import ExperienciaComponente from './components/ExperienciaComponente.vue'

import { onMounted, onUnmounted } from 'vue' 
import confetti from 'canvas-confetti'

let confettiInterval = null; 

// Función que lanza una ráfaga de confeti "cayendo"
function launchRain() {
  confetti({
    particleCount: 15,
    angle: 90,
    spread: 180,
    origin: { x: Math.random(), y: -0.1 },
    gravity: 0.4,
    disableForcibles: true, 
    scalar: 1.1,
    ticks: 300,
    drift: Math.random() < 0.5 ? -0.1 : 0.1
  });
}

onMounted(() => {
  confettiInterval = setInterval(launchRain, 80);
});

onUnmounted(() => {
  clearInterval(confettiInterval);
});

// Dispara el confeti cuando el componente se carga
onMounted(() => {
  confetti({
    particleCount: 450, // Cantidad de confeti
    spread: 100,
    origin: { y: 0.6 },
  });
});

</script>
