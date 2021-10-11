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
@import '~@fortawesome/fontawesome-free/scss/fontawesome';

button{
  min-width: 270px;
  min-height: 60px;
  border-radius: 2.8125rem;
  color: $primary_btn_color;
  background-color: $primary_btn_background_color;
  border: 0;
  margin: 0 15px;
}


#app {
  
  .page-margins{
    width: 70%;
    margin: auto;


  }

}
</style>
