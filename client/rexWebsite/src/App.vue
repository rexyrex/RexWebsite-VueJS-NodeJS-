<template>
  <div id="App">
    <titlez></titlez>
    <navbar></navbar>
    <router-view/>
    <footerz></footerz>
    
  </div>
</template>

<script>
import navbar from './components/NavBar' 
import titlez from './components/Title'
import footerz from './components/Footer'

export default {
  name: 'App',
  components: {
    "navbar" : navbar,
    "titlez" : titlez,
    "footerz" : footerz,
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
