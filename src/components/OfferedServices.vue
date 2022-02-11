<template>
    <div class="offered-services">
        <div class="dream">
            <text-big-dream/>
            <h2 class="tac fw-600">We are pioneers of the digital approach, using leading-edge</h2>
            <h2 class="tac fw-600">technology to simplify procedures and apply executive</h2>
            <h2 class="tac fw-600">coaching in the new age of digitalization</h2>
        </div>
        <div class="services ">
           <div class="card-service" v-for="cardService in cardsService" :key="cardService.id">
            <h2 class="pb-15 fw-600">{{cardService.title}}</h2>
            <p>{{cardService.text1}}</p>
            <p>{{cardService.text2}}</p>
            <p>{{cardService.text3}}</p>          
            </div>
        </div>
            <div class="button-cta pb-5">
                <div class="cta-learn-more">
                    Get started today
                </div>
                <button-cta/>
            </div> 
    </div>
</template>

<script>
import ButtonCta from './ButtonCta.vue'
import TextBigDream from './TextBigDream.vue'

export default {
    components:{ButtonCta ,TextBigDream },
    props:{
   
             cardsService:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .offered-services{
        .button-cta{
            display: flex;
            width: 100%;
            justify-content: center;
            padding-bottom: 30px;
             .cta-learn-more{
                color:$jungle-green-v ;
                background-color:$white ;
                width: 150px;
                height: 40px;
                line-height: 40px;
                font-size: 12px;
                text-align: center;
                border-radius: 2px;
                cursor: pointer;
                border: 1px solid grey;
                margin-right: 50px;
            }
        }
        .services{
            padding-top: 50px;
            display: flex;
            flex-wrap: wrap;
            // column-gap: 60px;
            row-gap: 50px;
            padding-bottom: 30px;
            padding-left: 140px;
            justify-content: center;
            width: 1200px;
            margin: 0 auto;
            .card-service{
                width: 321px;
                p{
                    color: $boulder;
                }
            }
        }
    }
</style>