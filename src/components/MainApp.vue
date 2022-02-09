<template>
    <div>
         <jumbotron/>
         <offered-services/>
         <program-coach/>
         <jumbotron-explore/>
    </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import OfferedServices from './OfferedServices.vue'
import ProgramCoach from './ProgramCoach.vue'
import JumbotronExplore from './JumbotronExplore.vue'
export default {
    components:{Jumbotron, OfferedServices, ProgramCoach,JumbotronExplore}
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
</style>