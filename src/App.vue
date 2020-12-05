<template>
  <div id="app">

    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <Noticias msg="Welcome to Your Vue.js App"/>
    <Integrantes msg="Welcome to Your Vue.js App"/>
    <Footer msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Footer from './components/Footer.vue'
import Integrantes from './components/Integrantes.vue'
import Noticias from './components/Noticias.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    Footer,
    Integrantes,
    Noticias,

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
