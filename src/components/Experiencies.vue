<script setup>
import Experiencie from "./experiencies/experiencie.vue";
</script>

<template>
  <div class="experiencies">
    <h2 class="title">Experiencies</h2>
    <ul class="experiencies-list">
      <Experiencie />
      <Experiencie />
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
