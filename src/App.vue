<template>
 
  <router-view/>
  <NavBar :logo="logo_src" alt="app_name"/>
  <Footer/>
  
</template>
<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'

export default{
  
    components:{ 
      NavBar,
      Footer
    },
    data(){
      return{
        logo_src: "/img/logo.png",
        alt: "Make Your Burger "
      }
    }
}

</script>


<style>

</style>
