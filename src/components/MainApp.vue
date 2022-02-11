<template>
    <div>
         <jumbotron/>
         <offered-services 
            :cardsService="cardsService"
         />
         <jumbotron-explore
            :jumboExplore="jumboExplore"
         />
         <price-services/>
         <youtube-video/>
         <upcoming-events
            :events="events"
         />
    </div>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import OfferedServices from './OfferedServices.vue'
import JumbotronExplore from './JumbotronExplore.vue'
import PriceServices from './PriceServices.vue'
import YoutubeVideo from './YoutubeVideo.vue'
import UpcomingEvents from './UpcomingEvents.vue'
export default {
    components:{Jumbotron, OfferedServices,JumbotronExplore,PriceServices, YoutubeVideo, UpcomingEvents},
    props:{
        cardsService:Array,
        jumboExplore:Array,
        events:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
</style>