<script setup>
defineProps({
  image: String,
  title: String,
  description: String,
  tecnologies: Array,
});
</script>

<template>
  <li class="experiencie">
    <div class="img"><img :src="image" alt="_img" /></div>
    <h3 class="title">{{ title }}</h3>
    <div class="tecnologies">
      <ul class="tecnologies-list">
        <li class="tecnologie" v-for="t in tecnologies" :key="t.title">
          <img
            :src="t.src"
            :alt="t.title"
            :title="t.title"
            width="30"
            height="30"
          />
        </li>
      </ul>
    </div>
    <p class="description">
      {{ description }}
    </p>
  </li>
</template>

<style scoped>
.experiencie {
  max-width: 500px;
  display: flex;
  gap: 1em;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.img {
  cursor: pointer;
  width: 150px;
  height: 150px;
  background-color: var(--bandito-yellow-color);
  clip-path: polygon(50% 0, 100% 20%, 100% 80%, 50% 100%, 0 80%, 0 20%);
}

.img img {
  width: 100%;
  height: 100%;
}

.tecnologies-list {
  list-style: none;
  display: flex;
  gap: 10px;
}

.tecnologie {
  cursor: pointer;
}

.description {
  text-align: center;
}
</style>
