<template>
  <div id="app">
    <Header :headerNavigationList="navListHeader"/>
    <Main/>
    <Footer :footerData="footerInformations"/>
  </div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';
import Footer from './components/Footer';
import '@fortawesome/fontawesome-free/js/all.js';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data(){
    return{
      navListHeader:[
        {
          name:'Home',
          link:'#',
          state:false,
        },
        {
          name:'Services',
          link:'#',
          state:false,
        },
        {
          name:'About',
          link:'#',
          state:false,
        },
        {
          name:'Videos',
          link:'#',
          state:false,
        },
        {
          name:'Blog',
          link:'#',
          state:false,
        },
        {
          name:'Store',
          link:'#',
          state:true,
        },
      ],
      footerInformations:{
        footerLinksList:[
          {
            name:'fab fa-facebook-f',
            link:'#',
          },
          {
            name:'fab fa-twitter',
            link:'#',
          },
          {
            name:'fab fa-youtube',
            link:'#',
          },
          {
            name:'fab fa-instagram',
            link:'#',
          },
          {
            name:'fab fa-linkedin',
            link:'#',
          },
          
        ],
        recentPostsList:[
          {
            content:'The best protein shake',
            link:'#'
          },
          {
            content:'Ultimate cardio Workout',
            link:'#'
          },
          {
            content:'New juices available now',
            link:'#'
          },
          {
            content:'Tips to find training partners',
            link:'#'
          },
          {
            content:'20 best healthy recipes',
            link:'#'
          },
        ],
        contactInfo:{
            address:'4746 Tipple Road Michigan 48449',
            mobilePhone:'1.800.000.0000',
            email:'info@your-company.com',
          },
      }
    }
  }
}
</script>

<style lang="scss">

@import './assets/style/general';
@import './assets/style/variables.scss';
@import '~@fortawesome/fontawesome-free/scss/fontawesome';


#app {
  
  .page-margins{
    width: 80%;
    margin: auto;

  }

}
</style>
