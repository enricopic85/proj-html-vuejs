<template>
    <div class="price-services">
        <text-big-dream/>    
        <help-you/>
        <div class="container-price">
            <div class="card-price">
                
            </div>
            <div class="card-price1"></div>
            <div class="card-price2"></div>
            <div class="card-price3"></div>
            <div class="card-price4"></div>
        </div>
    </div>
</template>

<script>
import HelpYou from './HelpYou.vue'
import TextBigDream from './TextBigDream.vue'
export default {
    components:{TextBigDream, HelpYou}
}
</script>

<style lang=
"scss" scoped>
@import '@/../style/variables.scss';
    .price-services{
        width: 100%;
        height: 550px;
       .container-price{
           display: flex;
           padding-top: 30px;
           justify-content: center;
           gap: 30px;
           .card-price1,.card-price2,.card-price3,.card-price4{
               width: 280px;
               height: 350px;
               border: 1px solid black;
                border-radius: 5px;
                 background-size: cover;
           }
           .card-price1,.card-price4{
               background-image: url('/img/stock-full-hd-03-443x600.jpg');
            }
           .card-price2{
               background-image: url('/img/stock-full-hd-04-443x600.jpg');
           }
           .card-price3{
               background-image: url('/img/stock-full-hd-06-443x600.jpg');
           }

       }
    }
</style>