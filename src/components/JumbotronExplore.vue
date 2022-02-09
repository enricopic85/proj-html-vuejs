<template>
    <div class="jumbotron-explore">
        <div class="explore">
            <h4>Let's Dream Big Together</h4>
            <h2>Explore How can I help you</h2>
            <div class="container-explore">
                <div class="card-explore">
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
                </div>
                 <div class="card-explore">
                    <div class="explore-img">
                        <img src="/img/home-business-service-slide-02-480x298.jpg" alt="">
                    </div>
                    <h3>Real Deal Coaching</h3>
                    <p>Bring an exceptionally powerful</p>
                    <p>opportunity. Being able to accept, to work</p>
                    <p class="pb-30">with that opportunity</p>
                    <div class="discover-now">
                        Discover now ->
                    </div>
                </div>
                <div class="card-explore">
                    <div class="explore-img">
                        <img src="/img/home-business-service-slide-03-480x298.jpg" alt="">
                    </div>
                    <h3>Advisor Training Program</h3>
                    <p>Getting high quality, entrepreneur mindset</p>
                    <p>driven online business coaching, is what is</p>
                    <p class="pb-30">needed</p>
                    <div class="discover-now">
                        Discover now ->
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

export default {
    
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
            padding-left: 675px;
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
             padding-top: 50px;
           h4{
            color: $jungle-green;
            padding-bottom: 15px;
           }
        }
        .container-explore{
            padding-top: 30px;
            padding-left: 110px;
            padding-bottom: 30px;
            display: flex;
            gap: 30px;
            justify-content: center;
            
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