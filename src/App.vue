<template>
<Navbar/>
<router-view/>
<Footer/>
<div class="icons">
<a href="https://www.instagram.com/leonard_beyonce/" target="_blank"><i class="fa fa-instagram" aria-hidden="true"></i></a>
<a href="https://twitter.com/beyonce_leonard" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a>
<a href="https://www.facebook.com/beyonce.leonard.39" target="_blank"><i class="fa fa-facebook-official" aria-hidden="true"></i></a> 
</div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'
export default {
  components:{
    Navbar,Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  font-size: 25px;
  color: #080808;
  text-decoration: none;
}

nav a.router-link-exact-active {
  color: #3f9be1;
}
.icons{
  font-size: 25px;
}
</style>
