<template>
  <div id="app">
    <div class="main-container">
      <NavMenu />
      <router-view /> 
      <Footer />
    </div>
  </div>
</template>

<script>
import NavMenu from './components/NavMenu.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NavMenu,
    Footer
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');

  body {
    margin: auto;
  }

  #app {
    font-family: 'Roboto', sans-serif;
    text-align: center;
  }

  .main-container {
    display: flex;
    flex-direction: column;
  }
</style>
