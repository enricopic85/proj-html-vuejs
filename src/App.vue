<template>
  <div id="app">
    <header-app 
    :menu="menu"
    :languages="languages"/>
    <main-app />
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
   
  },
  data(){
    return{
      menu:['Home','Pages','Courses','Features','Blog','Shop'],
      languages:[
        {
          id:1,
          img:'@/../public/img/fr.png',
          nation:'FRANCE'
        },
        {
          id:2,
          img:'@/../public/img/de.png',
          nation:'GERMANY'
        },
      ]
    }
  },
  
}
</script>

<style lang="scss">
  @import './style/main.scss';
  @import '@/../style/variables.scss';
</style>
