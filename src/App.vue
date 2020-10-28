<template>
  <div id="app" v-on:mousemove="followCursor">
    <Navigation/>
    
    <router-view></router-view>
    <!-- <span id="circle" class="circle"></span>-->
 

    <Home/>
  </div>
  
</template>

<script>
import Home from './components/Home/Home.vue'
import Navigation from './components/Used/Navigation.vue'

export default {
  name: 'App',
  props:{

  },
  components: {
    Home,
    Navigation,
  },

  methods:{
    followCursor: function(e){
      var x = e.clientX;
      var y = e.clientY;
      e = (x + ' ' + y); 
    }
  },

  data(){
    return{
        
    }
  }
};
</script>

<style>
#app {
  position: relative;
  font-family: quicksand;
  background: linear-gradient(-0.02turn, #ffffff 40%, #d1c9ff  );
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #5c5c5c;
}

.circle {
	position: absolute;
  border: solid 1px #ccc;
	width: 60px; 
	height: 60px; 
  border-radius: 50%;  
}
</style>
