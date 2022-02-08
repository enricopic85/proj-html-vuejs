<template>
    <div>
       <nav-bar :menu="menu"/>
       <jumbotron/>
    </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import NavBar from './NavBar.vue'
export default {
  components: { NavBar, Jumbotron },
  props:{
      menu:Array
  }
    
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
   
</style>