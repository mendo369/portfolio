<script setup></script>

<template>
  <div class="about-me">
    <div class="hello">
      <p class="hello-text">
        Hello <span class="dot">.</span>
        <br />
        I am Luis
      </p>
      <p class="presentation-text">
        Web developer with 1+ years of experience in frontend and backend
        development. Proven ability to create attractive and functional web
        interfaces using JavaScript, React, and Redux. Passionate about
        innovation and continuous learning, seeking to contribute to meaningful
        technological projects that help me grow professionally.
      </p>
    </div>
    <div class="img-container">
      <div class="img">
        <img src="../assets/images/1701098779912.jpg" alt="img" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.about-me {
  width: 80%;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2em;
  flex-wrap: wrap;
}

.hello {
  display: grid;
  gap: 1em;
  flex: 2;
}

.hello-text {
  font-size: 2em;
  font-weight: bold;
  height: min-content;
}

.presentation-text {
  font-size: medium;
}

.dot {
  color: var(--bandito-yellow-color);
  font-size: 1.5em;
  font-weight: bolder;
}

.img-container {
  flex: 1;
}

.img {
  min-width: 200px;
  max-width: 200px;
  min-height: 200px;
  max-height: 200px;
  border-radius: 50%;
  /* clip-path: polygon(
    20% 0%,
    80% 0%,
    100% 20%,
    100% 80%,
    80% 100%,
    20% 100%,
    0% 80%,
    0% 20%
  ); */
  overflow: hidden;
  background-color: var(--bandito-yellow-color);
}

.img {
  filter: grayscale(1);
  transition: all 0.5s;
  cursor: pointer;
}

.img:hover {
  filter: grayscale(0);
  /* box-shadow: 0px 0px 20px #fce30042; */
}
.img img {
  width: 100%;
  height: 100%;
  transition: all 0.5s;
}
.img:hover img {
  transform: scale(1.1);
}
</style>
