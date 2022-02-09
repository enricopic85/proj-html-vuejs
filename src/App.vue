<template>
  <div id="app">
    <header-app 
    :menu="menu"
    :languages="languages"/>
    <main-app
    :cardsService="cardsService" />
    <footer-app :listFooter="listFooter"/>
  </div>
</template>

<script>
import FooterApp from './components/FooterApp.vue'
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'



export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    FooterApp
   
  },
  data(){
    return{
      menu:['Home','Pages','Courses','Features','Blog','Shop'],
      languages:[
        {
          id:1,
          img:'/img/fr.png',
          nation:'FRANCE'
        },
        {
          id:2,
          img:'/img/de.png',
          nation:'GERMANY'
        },
      ],
      cardsService:[
        {
          id:1,
          title:'One to one',
          text1:'Getting the necessary clarity about the',
          text2:'current state to help you improve your',
          text3:'game'
        },
         {
          id:2,
          title:'Anywhere',
          text1:'Access to valuable and portable',
          text2:'program which allow you to setup and',
          text3:'live anywhere you want'
        },
         {
          id:3,
          title:'On Time',
          text1:'Punctuality is our top priority because it\'s  ',
          text2:'an essential criteria to assess a program',
          text3:'quality'
        },
         {
          id:4,
          title:'Online Courses',
          text1:'Online business coaching now offers you',
          text2:'a very powerful way to empower your',
          text3:'business into success'
        },
         {
          id:5,
          title:'Consulting',
          text1:'You will get a clear sense of direction for',
          text2:'your business, thorough assessment and',
          text3:'faster results'
        },
         {
          id:6,
          title:'Self Development',
          text1:'Business Coaching often keep your focus',
          text2:'and develop you both in a professional',
          text3:'and personal way'
        },
      ],
      listFooter:[
        {
          id:1,
          title:'Explore',
          link1:'Start here',
          link2:'blog',
          link3:'About us',
          link4:''
        },
        {
          id:2,
          title:'',
          link1:'Success story',
          link2:'Courses',
          link3:'Contact us',
          link4:''
        },
        {
          id:3,
          title:'Information',
          link1:'Membership',
          link2:'Purchase guide',
          link3:'Privacy policy',
          link4:'Terms of service'
        },
      ]
    }
  },
  
}
</script>

<style lang="scss">
  @import './style/main.scss';
  @import '@/../style/variables.scss';
</style>
