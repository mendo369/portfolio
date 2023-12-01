<script setup>
import proyects from "../data/proyects.json";
console.log(proyects);
import Proyect from "./proyects/proyect.vue";
</script>

<template>
  <div class="proyects" id="proyects">
    <h2 class="title">Proyects</h2>
    <ul class="proyects-list">
      <Proyect
        v-for="proyect in proyects"
        :key="proyect.name"
        :image="proyect.image"
        :name="proyect.name"
        :description="proyect.description"
        :url="proyect.url"
        :tecnologies="proyect.tecnologies"
      />
    </ul>
  </div>
</template>

<style scoped>
.proyects {
  width: 80%;
}

.title {
  margin-bottom: 1em;
}

.proyects-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1em;
}
</style>
