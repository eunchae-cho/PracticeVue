<template>
  <div id="app">
    <eunchae-header/>
    <eunchae-list/>
    <eunchae-footer/>
  </div>
</template>

<script>
import EunchaeHeader from './components/EunchaeHeader.vue'
import EunchaeFooter from './components/EunchaeFooter.vue'
import EunchaeList from './components/EunchaeList.vue'

export default {
  // name: 'App',
  components: {
    EunchaeHeader,
    EunchaeList,
    EunchaeFooter
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
