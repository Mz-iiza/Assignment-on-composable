<template>
  <div id="app">
    <ColorPickerGame />

  </div>
 
  <!--<HelloWorld msg="Welcome to Your Vue.js App"/> -->
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue' 

import ColorPickerGame from './components/ColorPickerGame.vue';


export default {
  name: 'App',
  components: {
    ColorPickerGame
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
