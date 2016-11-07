<template>
  <div id="app">
    <img src="./assets/logo.png">
    <global-header></global-header>
  </div>
</template>

<script>
import GlobalHeader from './components/GlobalHeader'

export default {
  name: 'app',
  components: {
    GlobalHeader
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

body{
  margin: 0px;
}
</style>
