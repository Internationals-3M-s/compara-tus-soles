<template>
  <NavComponent />
  <div class="container">
    <HeroSection />
  </div>
</template>

<script>
import NavComponent from "./components/NavComponent.vue"
import HeroSection from "./components/HeroSection.vue"

export default {
  name: 'App',
  components: {
    NavComponent,
    HeroSection,
}
}
</script>

<style>
#app {
  
  -webkit-font-smoothing: antialiased;
  /* -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px; */
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

</style>
