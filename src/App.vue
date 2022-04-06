<template>
  <div id="app">
    <HeaderSide />
    <MainSide />
    <FooterSide />
  </div>
</template>

<script>
import HeaderSide from './components/HeaderSide.vue';
import MainSide from './components/MainSide.vue';
import FooterSide from './components/FooterSide.vue';

export default {
  name: 'App',
  components: {
    HeaderSide,
    MainSide,
    FooterSide,
    
    
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
#app {
  width: 100%;
  height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; 
  display: flex;
  flex-direction: column;
}
</style>
