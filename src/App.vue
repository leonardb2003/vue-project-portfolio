<template>
  <div class="background">
<Navbar/>
<router-view/>
<Footer/>
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
.background{
  background-color: #042547;
  min-height: 100vh;
  min-width: 100vh;
}
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
</style>
