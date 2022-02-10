<template>
    <div class="price-services">
        <text-big-dream/>    
        <help-you/>
        <div class="container-price">
            <card-price-1/>
            <card-price-2/>
            <card-price-3/>
            <card-price-4/>
        </div>
    </div>
</template>

<script>
import CardPrice1 from './CardPrice1.vue'
import CardPrice2 from './CardPrice2.vue'
import CardPrice3 from './CardPrice3.vue'
import CardPrice4 from './CardPrice4.vue'
import HelpYou from './HelpYou.vue'
import TextBigDream from './TextBigDream.vue'
export default {
    components:{TextBigDream, HelpYou,CardPrice1, CardPrice2,CardPrice3,CardPrice4}
}
</script>
        
<style lang="scss" scoped>
@import '@/../style/variables.scss';
@import '@/../style/cardPrice.scss';
    .price-services{
        width: 100%;
        height: 600px;
       .container-price{
           display: flex;
           padding-top: 30px;
           justify-content: center;
           gap: 30px;
        }
    }
</style>