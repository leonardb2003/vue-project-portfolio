<template>
 <div data-aos="fade-down" data-aos-duration="3000" class="image">
  <img src="https://i.postimg.cc/2rN1L2T9/IMG-20211219-WA0025.jpg" width="400" height="500" id="image">
 </div> 
<div class="logo-name">
  <h1 data-aos="zoom-in" data-aos-duration="3000">Hello, I'm Beyonce Leonard</h1>
</div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import AOS from 'aos'


export default {
  name: 'HomeView',
  mounted() {
    AOS.init();
  },
  components: {
    HelloWorld
  }
}
</script>
<style>
.logo-name{
  font-size: 40px;
  font-weight: 500;
  color: #357fe0;
}
#image{
  /* background-repeat: no-repeat; */
  border-radius: 35px;
  margin-top: 30px;
}  
</style>

