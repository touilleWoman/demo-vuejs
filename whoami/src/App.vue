<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <whoami />
  </div>
</template>

<script>
import Whoami from './components/Whoami.vue'

export default {
  name: 'App',
  components: {
    Whoami
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
