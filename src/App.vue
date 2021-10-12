<template>
  <div id="app">
    <Header :headerNavigationList="navListHeader"/>
    <Main/>
    <Footer/>
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
      ]
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
