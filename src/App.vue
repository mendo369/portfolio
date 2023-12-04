<script setup>
import Header from "./components/Header.vue";
import AboutMe from "./components/AboutMe.vue";
import Proyects from "./components/Proyects.vue";
import Experiencies from "./components/Experiencies.vue";
import Education from "./components/Education.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <div class="main">
    <Header />
    <AboutMe />
    <Proyects />
    <Experiencies />
    <Education />
    <!-- <Footer /> -->
  </div>
</template>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  gap: 2em;
}
</style>
