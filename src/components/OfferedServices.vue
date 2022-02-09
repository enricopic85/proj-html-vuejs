<template>
    <div class="offered-services">
        <div class="dream">
            <h4 class="dreams">Let's Dream Big Together</h4>
            <h2 class="tac">We are pioneers of the digital approach, using leading-edge</h2>
            <h2 class="tac">technology to simplify procedures and apply executive</h2>
            <h2 class="tac">coaching in the new age of digitalization</h2>
        </div>
        <div class="services ">
           <div class="card-service" v-for="cardService in cardsService" :key="cardService.id">
            <h2 class="pb-15">{{cardService.title}}</h2>
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

export default {
    components:{ButtonCta , },
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
            padding-bottom: 50px;
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
       
        .dream{
            .dreams{
            padding-top: 50px;
            color: $jungle-green;
            text-align: center;
            padding-bottom: 15px;
        }
        }
        
        .services{
            padding-top: 50px;
            display: flex;
            flex-wrap: wrap;
            column-gap: 60px;
            row-gap: 50px;
            padding-bottom: 30px;
            padding-left: 208px;
            .card-service{
                width: 321px;
            }
        }
    }
</style>