<template>
    <div class="footer">
        <div class="footer-flex">
            <div class="address">
                <h5>Address</h5>
                <p>382 NE 191st St #87394 Miami, FL 33179-3899</p>
                <p>+1(305)547-9909(9am - 5pmEST,Monday-Friday)</p>
                <p>support@maxcoach.com</p>
                <div class="social">
                    <i class="fab fa-facebook-square"></i>
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-instagram"></i>
                    <i class="fab fa-linkedin"></i>
                </div>
            </div>
            <div class="footer-list">
                <div class="list" v-for="list in listFooter" :key="list.id" >
                    <h5 >{{list.title}}</h5>
                    <p>{{list.link1}}</p>
                    <p>{{list.link2}}</p>
                    <p>{{list.link3}}</p>
                    <p >{{list.link4}}</p>
                </div>
            </div>
        </div>
        <div class="copy">
            <i class="far fa-copyright"></i> 2020 Maxcoach. All Rights Reserved
        </div>
    </div>
</template>

<script>
export default {
    props:{
        listFooter:Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/../style/variables.scss';
    .footer{
        width: 100%;
        height: 300px;
        background-color: $tuna;
        .copy{
            color: $white;
            font-size: 12px;
            padding-top: 50px;
            text-align: center;
        }
        .footer-flex{
            display: flex;
            .address{
            color: $white;
            display: flex;
            flex-direction: column;
            padding-top: 50px;
            gap: 20px;
            padding-left: 200px;
            padding-right: 150px;
            p{
                font-size: 12px;
            }
            .social{
                display: flex;
                gap: 20px;
            }
        }
        .footer-list{
            display: flex;
            color: $white;
            padding-top: 50px;
            p{
                font-size: 12px;
            }
            .list{
                display: flex;
                flex-direction: column;
                padding-right: 40px;
                gap: 20px;
                h5{
                    height: 16px;
                }
            }
        }
        }
    }
</style>