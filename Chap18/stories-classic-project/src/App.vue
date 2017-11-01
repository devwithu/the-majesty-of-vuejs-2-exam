<template>
  <div id="app">
    <component :is="currentComponent"></component>
    <p>
      this is very useful...
    </p>
    <a href="#" @click="currentComponent = 'HelloWorld'">Show HelloWorld</a>
    <a href="#" @click="currentComponent = 'greet'">Show Greet</a>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Greet from './components/Greet'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Greet
  },
  data(){
    return {
      currentComponent: "HelloWorld"
    }
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
