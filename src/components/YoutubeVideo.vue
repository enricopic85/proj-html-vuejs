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
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
.youtube{
    background-color:  $charade; 
    height: 600px;
    display: flex;
    align-items: center;
    justify-content: center;
    .video{
        position: relative;
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
}
</style>