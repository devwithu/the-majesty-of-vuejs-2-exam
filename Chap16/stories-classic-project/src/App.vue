<template>
  <div id="app">
    <img src="./assets/logo.png">
    <!-- <HelloWorld/> -->
    <!-- <Login/> -->
    <register></register>
    <!-- <stories></stories> -->
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Login from './components/Login.vue'
import Register from './components/Register.vue'
import Stories from './components/Stories.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Login,
    Register,
    Stories
  },
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
