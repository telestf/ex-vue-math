<template>
  <div id="app">
    <HelloWorld msg="Meu primeiro Math App.js"/>
    <div class="container">
      <Fatorial :numero="9"/>
      <Primo :numero="13"/>
      <Quadrado :numero="2"/>
      <Cubo :numero="3"/>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Quadrado from './components/Quadrado.vue'
import Cubo from './components/Cubo.vue'
import Fatorial from './components/Fatorial.vue'
import Primo from './components/Primo.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    Quadrado,
    Cubo,
    Fatorial,
    Primo
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

.container {
  display: flex;
  justify-content: space-around;
}
</style>
