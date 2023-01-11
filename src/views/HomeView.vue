<template>  
  <img src="https://i.postimg.cc/2rN1L2T9/IMG-20211219-WA0025.jpg" width="400" height="500" id="image"> 
<div class="logo-name">
  <h1>Beyonce Leonard</h1>
</div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
<style>
.logo-name{
  font-size: 40px;
  font-weight: 500;
  color: rgb(0, 110, 255);
}
#image{
  /* background-repeat: no-repeat; */
  border-radius: 35px;
  margin-top: 30px;
}  
</style>

