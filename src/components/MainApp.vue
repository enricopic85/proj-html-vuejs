<template>
    <div>
         <jumbotron/>
         <offered-services/>
    </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import OfferedServices from './OfferedServices.vue'
export default {
    components:{Jumbotron, OfferedServices}
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
</style>