<script setup>
defineProps({
  image: String,
  name: String,
  description: String,
  url: String,
  tecnologies: Array,
});

const navigate = (url) => {
  window.open(url);
};
</script>

<template>
  <li class="proyect">
    <div class="gallery">
      <div
        class="img-main"
        @click="
          () => {
            navigate(url);
          }
        "
      >
        <img :src="image" alt="_img" />
        <!-- <iframe width="300" height="200" src="https://colrifas.netlify.app">
        </iframe> -->
      </div>
    </div>
    <div class="description">
      <h3 class="proyect-name">{{ name }}</h3>
      <p class="proyect-description">
        {{ description }}
      </p>
      <div class="icons-tecnologies">
        <ul class="list-icons-tecnologies">
          <li
            class="tecnology"
            v-for="tecnology in tecnologies"
            :key="tecnology.title"
          >
            <img
              :src="tecnology.src"
              alt="_tec"
              width="30"
              height="30"
              :title="tecnology.title"
            />
          </li>
        </ul>
      </div>
    </div>
  </li>
</template>

<style scoped>
.proyect:nth-child(even) {
  flex-direction: row-reverse;
}

.proyect {
  /* border: 1px solid white; */
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 1em;
  width: 90%;
  align-items: center;
  justify-content: center;
}

.gallery {
  min-width: 300px;
  min-height: 300px;
  display: flex;
  align-items: center;
}

.img-main {
  overflow: hidden;
  background-color: var(--bandito-yellow-color);
  width: 300px;
  height: 200px;
  margin: auto;
  border-radius: 5px;
  box-shadow: 0px 2px 5px #fce300;
  cursor: pointer;
}

.img-main img {
  width: 100%;
  height: 100%;
}

.description {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 1em;
  min-width: 300px;
}

.proyect-name {
  color: var(--bandito-yellow-color);
  letter-spacing: 2px;
  font-size: x-large;
}

.icons-tecnologies {
}

.list-icons-tecnologies {
  list-style: none;
  display: flex;
  gap: 1em;
}

.tecnology {
  width: 30px;
  height: 30px;
  cursor: pointer;
  border-radius: 5px;
  color: var(--vulture-black-color);
}
</style>
