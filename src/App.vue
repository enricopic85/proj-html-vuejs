<template>
  <div id="app">
    <header-app 
    :menu="menu"
    :languages="languages"/>
    <main-app
    :cardsService="cardsService"
    :jumboExplore="jumboExplore"
    :events="events" />
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
      ],
     jumboExplore:[
       {
         id:1,
         img:'home-business-service-slide-01-480x298.jpg' ,
         title:'Consultative training',
         text1:'With a coach addressing multiple issues',
         text2:'that are off balance, affecting your',
         text3:'business in various unconsidered ways'
       },
        {
         id:2,
         img:'home-business-service-slide-02-480x298.jpg' ,
         title:'Real Deal Coaching',
         text1:'Bring an exceptionally powerful',
         text2:'opportunity. Being able to accept, to work',
         text3:'with that opportunity'
       },
        {
         id:3,
         img:'home-business-service-slide-03-480x298.jpg' ,
         title:'Advisor Training Program',
         text1:'Getting high quality, entrepreneur mindset',
         text2:'driven online business coaching, is what is',
         text3:'needed'
       },

     ],
     events:[
       {
         id:1,
         location:'Texas, US',
         title:'Storytelling Workshop',
         day:'22',
         month:'NOV'
       },
       {
         id:2,
         location:'New York, US',
         title:'Painting Art Contest 2020',
         day:'10',
         month:'OCT'
       },
       {
         id:3,
         location:'Hambur, Germany',
         title:'International Art Fair 2020',
         day:'23',
         month:'NOV'
       },
       {
         id:4,
         location:'Illinois, US',
         title:'Street Performance: Call for Artist',
         day:'15',
         month:'DEC'
       },
       {
         id:5,
         location:'Illinois, US',
         title:'Consumer Food Safety Education Conference',
         day:'22',
         month:'JUL'
       },
       {
         id:6,
         location:'Dubai',
         title:'How meditation improve your mental health?',
         day:'12',
         month:'AUG'
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
