<script setup>
</script>

<template>
  <section class="datos-personales">
    <div class="card">
      <h1>Maximiliano A Morales</h1>
      <h2>Técnico Universitario en programacion - utn</h2>
      <p>Hola, Bienvenido a mi portafolio de proyectos. Soy estudiante en programacion</p>
      <ul class="container-lista">
        <li v-for="red in redesSociales" :key="red.id">
          <a :href="red.url"><img class="icon-redsocial" :src="red.src" width="35rem" :alt="red.name"></a>
        </li>
      </ul>
      <h3>☎ Mi Teléfono personal: {+5492984661349</h3>
      <h4>Gral. Roca, RN</h4>
    </div>
  </section>
</template>

<style scoped>

</style>