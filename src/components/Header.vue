<script setup></script>

<template>
  <nav class="nav">
    <div class="title"><h1>Luis David Mendoza</h1></div>
    <div class="navigation">
      <ul class="navigation-list">
        <li>Me</li>
        <li>Proyect</li>
        <li>Github</li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.nav {
  background-color: var(--bandito-yellow-color);
  /* position: absolute;
  top: 0;
  left: 0; */
  width: 100%;
  color: var(--vulture-black-color);
  font-weight: bold;
  display: flex;
  justify-content: space-between;
  padding: 10px 20px;
  align-items: center;
}

.navigation-list {
  list-style: none;
  display: flex;
  flex-wrap: nowrap;
  gap: 10px;
}
</style>
