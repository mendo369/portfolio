<script setup></script>

<template>
  <div class="education">
    <h2 class="title">Education</h2>
    <ul class="education-list">
      <li class="education-item">
        <img class="img" src="/images/Univalle.png" alt="_img" />
        <h3>Universidad del Valle</h3>
      </li>
      <li class="education-item">
        <img class="img" src="/images/uis.png" alt="" />
        <h3>Universidad Industrial de Santander / MinTic</h3>
      </li>
      <li class="education-item">
        <img class="img" src="/images/udemy.png" alt="" />
        <h3>Udemy</h3>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.education {
  margin: 1em 0;
  width: 80%;
  min-height: 200px;
}

.img {
  width: 40px;
  height: 45px;
  padding: 1px;
  border-radius: 5px;
  /* background-color: var(--bandito-yellow-color); */
}

.title {
  margin-bottom: 1em;
  text-align: end;
}

.education-list {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1em;
}

.education-item {
  width: max-content;
  display: flex;
  align-items: center;
  gap: 5px;
}
</style>
