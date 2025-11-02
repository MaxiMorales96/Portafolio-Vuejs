<template>
  <div>
    <header>
      <h2>Maximiliano A Morales</h2>
      <nav>
        <a href="#">Inicio</a>
        <a href="#sobre">Sobre mí</a>
        <a href="#proyectos">Portafolio</a>
        <a href="#experiencia">Experiencia</a>
        <a href="#contacto">Contacto</a>
      </nav>
    </header>

    <section class="hero">
      <div class="hero-text">
        <p>Hola, soy</p>
        <h1>Maximiliano A Morales</h1>
        <p>Actualmente estudio Programación en la UTN, impulsado por mi interés en la tecnología. Además de mi formación, cuento con experiencia práctica en la reparación de celulares.</p>
        <button>Sobre mí</button>
        <div class="socials">
          <a href="https://www.linkedin.com/in/maxi-morales-9b4541393/" target="_blank"><img src="./assets/linkedin.svg" alt="LinkedIn" /></a>
          <a href="https://github.com/MaxiMorales96" target="_blank"><img src="./assets/github.svg" alt="GitHub" /></a>
          <a href="https://www.instagram.com/m.a.mor712/" target="_blank"><img src="./assets/instagram.svg" alt="Instagram" /></a>
        </div>
      </div>
      <img src="./assets/photo.jpg" alt="Foto de Maximiliano A Morales" />
    </section>

    <section id="proyectos" class="proyectos">
      <div class="linea-decorativa">
        <div></div><div></div><div></div><div></div><div></div>
      </div>
      <h2>Proyectos</h2>
      <ProyectosComponente />
    </section>

    <section id="experiencia">
      <ExperienciaComponente />
    </section>
  </div>
</template>

<script setup>
import ProyectosComponente from './components/ProyectosComponente.vue'
import ExperienciaComponente from './components/ExperienciaComponente.vue'
</script>
