<template>
    <div class="offered-services">
        <div class="dream">
            <h4 class="dreams">Let's Dream Big Together</h4>
            <h2 class="tac">We are pioneers of the digital approach, using leading-edge</h2>
            <h2 class="tac">technology to simplify procedures and apply executive</h2>
            <h2 class="tac">coaching in the new age of digitalization</h2>
        </div>
        <div class="services ">
            <card-service/>
            <card-service/>
            <card-service/>
            <card-service/>
            <card-service/>
            <card-service/>
        </div>
            <div class="button-cta ">
                <div class="cta-learn-more">
                    Get started today
                </div>
                <button-cta/>
            </div> 
    </div>
</template>

<script>
import ButtonCta from './ButtonCta.vue'
import CardService from './CardService.vue'
export default {
    components:{ButtonCta , CardService}
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .offered-services{
        .button-cta{
            display: flex;
            width: 100%;
            justify-content: center;
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
            width: 1500px;
            column-gap: 60px;
            row-gap: 50px;
            padding-bottom: 30px;
            padding-left: 208px;
        }
    }
</style>