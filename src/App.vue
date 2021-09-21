<template>
  <div>
    <!-- <Greet Uname="AAA" color="red"/>
    <Greet Uname="VVV" color="blue"/>
     <Greet :Uname="name" color="green"/> -->
     <Article title="FCB" :likes="1000" :isQualified="false"/>
  </div>


</template>

<script>
// import Greet from './components/Greet.vue'
import Article from './components/Article.vue'


export default {
  name: 'App',
  components:{Article},
  data(){
    return{
    name:"Adarsh"
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
