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
    <div class="img"><img src="" alt="_img" /></div>
    <h3 class="title">Title</h3>
    <div class="tecnologies">
      <ul class="tecnologies-list">
        <li class="tecnologie">item</li>
        <li class="tecnologie">item</li>
        <li class="tecnologie">item</li>
      </ul>
    </div>
    <p class="description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur
      aliquam veritatis, distinctio aspernatur facilis voluptas numquam sed
      perferendis, saepe vero maxime quidem quae cumque accusamus soluta
      asperiores sapiente. Assumenda, sapiente?
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

.tecnologies-list {
  list-style: none;
  display: flex;
  gap: 10px;
}
</style>
