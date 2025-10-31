<script setup>
import icono1 from '/src/assets/imagen.svg';

import { ref } from 'vue';
const titulo = 'Técnico en Celulares';
const fecha = 'Desde Enero 2020 / Hasta Octubre 2025 ';
const experiencias = ref([
    { id: 1, src: icono1, parrafo: 'Me especializo en el diagnóstico y reparación avanzada de placas base (PCB) de dispositivos móviles. Mi enfoque va más allá del reemplazo de módulos; me centro en la microsoldadura de precisión y la reparación a nivel componente. Utilizando análisis de esquemáticos y equipamiento de diagnóstico, abordo fallas complejas que otros centros consideran irreparables. Mi trabajo se centra en la ingeniería inversa para aislar y solucionar el problema de raíz, restaurando la funcionalidad completa del dispositivo.' },
]);
</script>

<template>
    <div class="card">
        <h3 class="titulo">{{ titulo.toLocaleUpperCase() }}</h3>
        <p class="fecha">{{ fecha }}</p>
        <ul class="listado">
            <li class="item" v-for="experencia in experiencias" :key="experencia.id">
                <img class="imagen-svg" :src="experencia.src" width="45rem" :alt="experencia.parrafo">
                <p>{{ experencia.parrafo }}</p>
            </li>

            <!-- <li class="item"><img class="imagen-svg" src="/src/assets/imagen.svg" width="45rem" alt="">
                <p>Me especializo en dar vida a dispositivos que otros dan por perdidos. Mi fortaleza es la microelectrónica: diagnostico y reparo fallas a nivel componente que la mayoría no puede ver.</p>
            </li> -->
        </ul>
    </div>
</template>

<style scoped>
.card {
    display: flex;
    flex-direction: column;
    padding: 2rem;
    background-color: rgb(28, 41, 52);
    border-radius: 15px;
}

.titulo {
    font-size: 1.5rem;
    color: coral;
}

.fecha {
    font-size: 1rem;
    color: burlywood;
    margin-bottom: 1rem;
}

.listado {
    display: flex;
    flex-direction: column;
}

.item {
    align-items: center;
    display: flex;
    padding: 1rem;
    gap: 1.5rem;
}
</style>