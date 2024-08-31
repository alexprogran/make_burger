<template>  
  <NavBar :logo="logo_src" :alt="alt"/>
  <router-view/>
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
 *{
font-family: Helvetica;
/* padding: 0; */
margin: 0; 
box-sizing: border-box;
}

.main-container{
  
  margin: 85px;
  min-height: 250px;
}

h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}


</style>