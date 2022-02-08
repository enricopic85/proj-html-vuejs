<template>
    <div>
       <nav-bar :menu="menu"/>
    </div>
</template>

<script>
import NavBar from './NavBar.vue'
export default {
  components: { NavBar },
  props:{
      menu:Array
  }
    
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
   
</style>