<template>
  <div>
    <Header /> 
  </div> 
</template>

<script>
import Header from './components/Header.vue';
import './App.css'
export default {
  name: 'App',
  components: { Header },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
