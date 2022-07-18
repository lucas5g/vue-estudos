<template>
  <div id="app">
    <input type="text" placeholder="cpf" 
    v-mask="'###.###.###.##-##'">
    <br>

    <input v-mask="'##/##/####'" v-model="data"/>
    <br>
    <button 
      v-on:click="count++"
    >
      Clicou {{ count }} vezes 
    </button>
    <p>
      {{ count }}
    </p>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import VueMask from 'v-mask'
// import Vue from 'vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
  },
  data: () => {
    return {
      count: 0

    }
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
