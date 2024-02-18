

<script setup>
  import { ref } from "vue"
  import NavBar from "./components/NavBar.vue"
  import Resume from "./components/Resume.vue"
  import Projects from "./components/Projects.vue"
  import About from "./components/About.vue"

  import Landing from "./components/Landing.vue"

  const currentPage = ref("LANDING")

  function changePage(newPage) {
    currentPage.value = newPage
  }
</script>

<template>
  <NavBar @changePage="changePage"></NavBar>
  <div class="main">
    <Landing v-if="currentPage == 'LANDING'"></Landing>
    <Resume v-else-if="currentPage == 'RESUME'"></Resume>
    <Projects v-else-if="currentPage == 'PROJECTS'"></Projects>
    <About v-else-if="currentPage == 'ABOUT'"></About>
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
