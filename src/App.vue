<template>
  <div id="app">
    <HeaderSide />
  </div>
</template>

<script>
import HeaderSide from './components/HeaderSide.vue'
import MainSide from './components/MainSide.vue'
import FooterSide from './components/FooterSide.vue'

export default {
  name: 'App',
  components: {
    HeaderSide,
    
    
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  
  color: #2c3e50;
  margin-top: 60px;
}
</style>
