<template>
    <div>
         <jumbotron/>
         <offered-services 
         :cardsService="cardsService"/>
         <program-coach/>
         <jumbotron-explore
         :jumboExplore="jumboExplore"/>
         <price-services/>
         <youtube-video/>
    </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import OfferedServices from './OfferedServices.vue'
import ProgramCoach from './ProgramCoach.vue'
import JumbotronExplore from './JumbotronExplore.vue'
import PriceServices from './PriceServices.vue'
import YoutubeVideo from './YoutubeVideo.vue'
export default {
    components:{Jumbotron, OfferedServices, ProgramCoach,JumbotronExplore,PriceServices, YoutubeVideo},
    props:{
        cardsService:Array,
        jumboExplore:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
</style>