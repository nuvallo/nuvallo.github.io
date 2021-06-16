<template>
  <div>
    <Header />
    <div className="grid">
      <Sidebar />
      <Content />
    </div>
  </div>
  
</template>

<script>
import Header from './components/Header.vue';
import Sidebar from './components/Sidebar.vue';
import Content from './components/Content.vue';
import './App.css'
export default {
  name: 'App',
  components: { Header, Sidebar, Content },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.grid {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
