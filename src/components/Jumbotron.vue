<template>
    <div class="jumbo">
        <div class="started-today">
            <h4 class="pb-15">New Challenges,New Skills</h4>
            <h1>BUILD YOUR OWN </h1>
            <h1>LIFE COACHING </h1>
            <h1 class="pb-15">BUSINESS</h1>
            <p>Whole-life business Coaching for committed</p>
            <p class="pb-15">entrepreneurs</p>
            <div class="cta">
                Get started today
            </div>
        </div>
        <div class="business-man">
            <div class="coach">
                <img src="@/../public/img/home-business-hero-avatar.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
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
        // justify-content: center;
        .started-today{
            padding-left: 300px;
            padding-right: 100px;
            h4{
                color: $jungle-green;
            }
            .cta{
                color: $white;
                background-color: $jungle-green-v;
                width: 150px;
                height: 40px;
                line-height: 40px;
                font-size: 12px;
                text-align: center;
                border-radius: 2px;
                cursor: pointer;
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
            }
    }
</style>