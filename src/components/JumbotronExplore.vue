<template>
    <div class="jumbotron-explore">
        <div class="explore">
            <h4>Let's Dream Big Together</h4>
            <h2>Explore How can I help you</h2>
            <div class="container-explore">
                <card-explore/>
                <card-explore/>
                <card-explore/>
                <!-- <div class="card-explore">
                    <div class="explore-img">
                        <img src="/img/home-business-service-slide-01-480x298.jpg" alt="">
                    </div>
                    <h3>Consultative training</h3>
                    <p>With a coach addressing multiple issues</p>
                    <p>that are off balance, affecting your</p>
                    <p class="pb-30">business in various unconsidered ways</p>
                    <div class="discover-now">
                        Discover now ->
                    </div>
                </div> -->
                 
            </div>
        </div>
    </div>
</template>

<script>
import CardExplore from './CardExplore.vue'
export default {
    components:{CardExplore}
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
.jumbotron-explore{
     background-color: $porcelain;
        height: 600px;
        width: 100%;
        .explore{
            text-align: center;
             padding-top: 50px;
           h4{
            color: $jungle-green;
            padding-bottom: 15px;
           }
        }
        .container-explore{
            padding-top: 30px;
            padding-left: 122px;
            padding-bottom: 30px;
            display: flex;
            gap: 30px;
            justify-content: center;
            // .card-explore{
            //     width: 350px;
            //     height: 400px;
            //     border: 1px solid black;
            //     border-radius: 2px ;
            //     h3{
            //         padding:20px 0;
            //     }
            //     .explore-img{
            //         width: 100%;
            //         height: 50%;
            //         img{
            //             width: 100%;
            //             height: 100%;
            //         }
            //     }
            //     .discover-now{
            //        color: $jungle-green;
            //        display: flex;
            //        align-items: center; 
            //        justify-content: center;
            //        height: 49px;
            //        font-weight: 800;
            //        border-top: 1px solid black;
            //         &:hover{
            //             color:$white;
            //             background-color: $jungle-green;
            //         }
            //     }
            // }
        }
}
</style>