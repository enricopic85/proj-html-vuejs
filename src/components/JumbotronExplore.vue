<template>
    <div class="jumbotron-explore">
        <div class="explore">
            <text-big-dream/>
            <help-you/>
            <div class="container-explore">
                <div class="card-explore" v-for="jumbo in jumboExplore" :key="jumbo.id">
                    <div class="explore-img">
                        <img :src="`/img/${jumbo.img}`" alt="">
                    </div>
                    <h3>{{jumbo.title}}</h3>
                    <p>{{jumbo.text1}}</p>
                    <p>{{jumbo.text2}}</p>
                    <p class="pb-30">{{jumbo.text3}}</p>
                    <div class="discover-now">
                        Discover now &#8702;
                    </div>
                </div>
            </div>
        </div>
         <div class="shot">
            <div class="shot-black"></div>
            <div class="shot-grey"></div>
            <div class="shot-grey"></div>
         </div>
    </div>
</template>

<script>
import HelpYou from './HelpYou.vue'
import TextBigDream from './TextBigDream.vue'

export default {
  components: { TextBigDream, HelpYou },
    props:{
        jumboExplore:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
.jumbotron-explore{
     background-color: $porcelain;
        height: 600px;
        width: 100%;
        .shot{
            display: flex;
            gap: 40px;
            padding-left: 13px;
            justify-content: center;
            .shot-black{
                width: 10px;
                height: 10px;
                border-radius: 50%;
                background-color: black;
                    }
            .shot-grey{
                width: 10px;
                height: 10px;
                border-radius: 50%;
                background-color: grey;
            }
                }
        .explore{
            text-align: center;
        }
        .container-explore{
            padding-top: 30px;
            padding-left: 100px;
            padding-bottom: 30px;
            display: flex;
            gap: 30px;
            justify-content: center;
            width: 1270px;
            margin: 0 auto;
            .card-explore{
                width: 350px;
                height: 400px;
                border: 1px solid black;
                border-radius: 2px ;
                p{
                   font-size: 14px;
                   font-weight: 500;
                }
                h3{
                    padding:20px 0;
                }
                .explore-img{
                    width: 100%;
                    height: 50%;
                    img{
                        width: 100%;
                        height: 100%;
                    }
                }
                .discover-now{
                   color: $jungle-green;
                   display: flex;
                   align-items: center; 
                   justify-content: center;
                   height: 52px;
                   font-weight: 800;
                   border-top: 1px solid black;
                    &:hover{
                        color:$white;
                        background-color: $jungle-green;
                    }
                }
                
            }
        }
}
</style>