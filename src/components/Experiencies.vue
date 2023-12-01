<script setup>
import experiencies from "../data/experiencies.json";
console.log(experiencies);
import Experiencie from "./experiencies/experiencie.vue";
</script>

<template>
  <div class="experiencies">
    <h2 class="title">Experiencies</h2>
    <ul class="experiencies-list">
      <Experiencie
        v-for="experiencie in experiencies"
        :key="experiencie.title"
        :image="experiencie.img"
        :title="experiencie.title"
        :description="experiencie.description"
        :tecnologies="experiencie.tecnologies"
      />
    </ul>
  </div>
</template>

<style scoped>
.experiencies {
  width: 80%;
}

.title {
  margin-bottom: 1em;
  text-align: center;
}

.experiencies-list {
  display: flex;
  gap: 3em;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  list-style: none;
}
</style>
