<template>
  <div id="app">
    <LandingPage />
  </div>
</template>

<script>
import LandingPage from './components/LandingPage.vue'

export default {
  name: 'app',
  components: {
    LandingPage
  }
}
</script>

<style>
#app {
  font-family: ibm-plex-sans, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #000;
}
</style>
