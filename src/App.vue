<template>
  <div>
    <!-- <Greet Uname="AAA" color="red"/>
    <Greet Uname="VVV" color="blue"/>
     <Greet :Uname="name" color="green"/> -->
     <!-- <Article id="my-article" title="FCB" :likes="1000" :isQualified="false"/> -->
     <button @click="visible=true">POP-UP</button>
     <popup v-show="visible" @close="close"/>
  </div>


</template>

<script>
// import Greet from './components/Greet.vue'
// import Article from './components/Article.vue'
import  popup  from "./components/popup.vue";


export default {
  name: 'App',
  components:{popup},
  data(){
    return{
      visible:false
    }
  },
  methods:{
    close(name){
      this.visible=false;
      console.log(name);
    }
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
  margin-top: 60px;
}

.danger {
  color:red;  
}

.cool{
  color:green;
}


</style>
