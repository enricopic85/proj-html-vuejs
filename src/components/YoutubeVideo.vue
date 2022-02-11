<template>
    <div class="youtube">
        <div class="video">
            <div class="content-video">
                <img src="/img/home-business-video-poster-670x450.jpg" alt="">
            </div>
            <div class="youtube-icon">
                <img src="/img/icon-youtube-play.png" alt="">
            </div>
        </div>
        <div class="good-plan">
            <h1>To Thrive in Business</h1>
            <h1>Today, You''ll Need a </h1>
            <h1>Good Plan</h1>
            <div class="answer">
                <h4 @click="flag(change)" class="pb-20"> <i class="fas fa-arrow-circle-down"></i> How can we help? </h4>
            </div>
            <div class="response" v-if="change">
                <p >How many courses you-ve been on, using however many techniques</p>
                <p>and methods. Unless you've come to realize the value of mindset, then</p>
                <p class="pb-20">you've to understand how success comes</p>
                <p>With everyone else's mindset involved impacting too, Hence why</p>
                <p class="pb-20">business coaching is so crucial for success</p>
            </div>
             <div class="hr "></div>
             <h4 class="pt-20 pb-20"> <i class="fas fa-arrow-circle-down "></i> Why would i need a business COACH?</h4>
             <div class="hr "></div>
             <h4 class="pt-20"> <i class="fas fa-arrow-circle-down "></i>    What is one-on-one coaching?</h4>
        </div>
        <div class="square">
            <img src="/img/maxcoach-shape-07.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            change:true
        }
    },
    methods:{
        flag(){ 
            this.change= !this.change
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
 @import './style/main.scss';
.youtube{
    background-color:  $charade; 
    height: 600px;
    display: flex;
    align-items: center;
    background-image: url('/img/background-map-dots-top-right-transparent.png');
    background-repeat: no-repeat;
    background-position: right;
    position: relative;
    justify-content: center;
    .square{
        width: 100px;
        height: 100px;
        position: absolute;
        z-index: 1;
        img{
            width: 100%;
        }
    }
    .video{
        position: relative;
        margin-left: 120px;
        z-index: 2;
         
        .content-video{
            width: 450px;
            height: 300px;
            border-radius: 5px;
            img{
                width: 100%;
                height: 100%;
                border-radius: 5px;
            }
        }
        .youtube-icon{
            width: 60px;
            height: 50px;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            img{
                width: 100%;
                height: 100%;
            }
        }
    }
    .good-plan{
        display: flex;
        flex-direction: column;
        padding-left: 60px;
        i{
                &:hover{
                     transform: rotate(180deg);
                   transition: 2s;
                }
            }
        h4{
            color: $white;
        }
        h1{
            color: $white;
        }
        p{
            color: $white;
        }
        .hr{
            border-bottom: 1px solid $white;
            width: 650px;
        }
        .answer{
            display: flex;
            gap: 15px;
            padding-top: 30px;
            h4{
                color: $mountain-meadow;
                cursor: pointer;
            }
            i{
               &:hover{
                   transform: rotate(180deg);
                   transition: 2s;
               }
            }
        }
        
    }
}
</style>