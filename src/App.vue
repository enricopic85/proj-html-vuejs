<template>
  <div id="app">
    <header-app/>
    <main-app/>
    <footer-app/>
  </div>
</template>

<script>
import FooterApp from './components/FooterApp.vue'
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'



export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    FooterApp
   
  }
}
</script>

<style lang="scss">
  @import './style/main.scss';
</style>
