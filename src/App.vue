<template>
  <div id="app">
    <Mylogo/>
    <Mycontainer/>
  </div>
</template>

<script>
import Mycontainer from './components/Mycontainer.vue';
import Mylogo from './components/Mylogo.vue'
export default {
  name: 'App',
  components: {
    Mycontainer,
    Mylogo
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>