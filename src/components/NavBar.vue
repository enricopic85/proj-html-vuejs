<template>
    <nav>
        <div class="logo">
            <img src="/img/dark-logo.png" alt="">
        </div>
        <ul>
            <li v-for="(list,i) in menu" :key="i">{{list}}
                <i class="fas fa-angle-down"></i>
            </li>
        </ul>
        <div class="language-search">
            <div class="language">
                <div class="flag">
                    <img src="/img/en.png" alt="">
                </div>
                <p>ENGLISH</p>
                <i @click="checked" class="fas fa-angle-down"></i>
                <i class="far fa-user-circle"></i>
            </div>
            <div class="modal-language" v-if="flag">
                <div class="language-card" v-for="language in languages" :key="language.id">
                <div class="flag">
                    <img :src=language.img alt="">
                </div>
                <p>{{language.nation}}</p>
            </div>
            </div>
            <div class="search">
                <input type="text" placeholder="Search...">
                <i class="fas fa-search"></i>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    props:{
        menu:Array,
        languages:Array,
    },
    data(){
        return{
            flag:false
        }
    },
    methods:{
        checked(){
            this.flag=!this.flag
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '@/../style/variables.scss';
    nav{
        display: flex;
        height: 80px;
        align-items: center;
        padding-left: 80px;
        justify-content: space-between;
        .logo{
            width: 140px;
            img{
                width: 100%;
               
            }
        }
        .language-search{
            display: flex;
            position: relative;
            .modal-language{
                display: flex;
                position: absolute;
                top:55px;
                z-index: 1;
                flex-direction: column;
                .language-card{
                     display: flex;
                    align-items: center;
                    padding-top: 20px;
                     
                }
                .flag{
                    padding-right: 5px;
                }
                i{
                    padding-left: 5px;
                }
            }
           
            .language{
                display: flex;
                align-items: center;
                border-right: 1px solid $porcelain;
                height: 80px;
                
                .flag{
                    padding-right: 5px;
                }
                 span{
                font-weight: 800;
                padding-left: 10px;
            }
            i{
                padding-left: 5px;
                padding-right: 20px;
                cursor: pointer;
            }
            }
            .search{
                align-items: center;
                display: flex;
                input{
                    height: 30px;
                    border: none;
                    margin-left: 20px;
                }
                i{
                    padding-right: 10px;
                }
            }
        }
        ul{
            display: flex;
            padding-left: 20px;
            li{
                list-style: none;
                padding-right: 30px;
               display: flex;
               align-items: self-end;
               color: $charade;
               font-size: 14px;
               font-weight: 600;
               i{
                   padding-left: 3px;
                    color: $tuna;
                    font-size: 12px;
                    line-height: inherit;
               }
            }
        }
    }
</style>