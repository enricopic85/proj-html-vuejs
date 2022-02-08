<template>
    <div class="jumbo">
        <div class="started-today">
            <h4 class="pb-15">New Challenges,New Skills</h4>
            <h1>BUILD YOUR OWN </h1>
            <h1>LIFE COACHING </h1>
            <h1 class="pb-15">BUSINESS</h1>
            <p>Whole-life business Coaching for committed</p>
            <p class="pb-15">entrepreneurs</p>
            <button-cta/>
        </div>
        <div class="business-man">
            <div class="coach">
                <img src="@/../public/img/home-business-hero-avatar.png" alt="">
            </div>
            <div class="action">
                <i class="fas fa-exclamation-triangle"></i>
                <i class="fas fa-globe"></i>
                <i class="fas fa-book"></i>
                <i class="fas fa-shopping-cart"></i>
            </div>
        </div>
    </div>
</template>

<script>
import ButtonCta from './ButtonCta.vue'
export default {
  components: { ButtonCta },
    
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .jumbo{
        background-color: $porcelain;
        height: 500px;
        background-image: url('/img/home-business-hero-global-image.png');
        background-size: contain;
        background-repeat: no-repeat;
        background-position: right;
        display: flex;
        align-items: center;
        position: relative;
        .started-today{
            padding-left: 300px;
            padding-right: 100px;
            h4{
                color: $jungle-green;
            }
        }
         .business-man{
                width: 300px;
                .coach{
                    width: 364px;
                    margin-top: 49px;
                    img{
                        width: 100%;
                    }
                }
                .action{
                    position: absolute;
                    display: flex;
                    flex-direction: column;
                    background-color: white;
                    width: 25px;
                    height: 130px;
                    justify-content: center;
                    gap: 10px;
                    align-items: center;
                    right: 0;
                    bottom: 349px;
                    border-radius: 2px;
                    
                }
                
            }
    }
</style>