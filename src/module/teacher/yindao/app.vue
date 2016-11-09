<template>

<ul>
  <li v-for='path in paths'>
    <img :src='path'>
  </li>
</ul>

</template>

<script>

import Lib from 'assets/Lib.js'


export default {
  data() {
    return {
      paths:[require('./cinema/yindao1.jpg'),require('./cinema/yindao2.jpg'),require('./cinema/yindao3.jpg')]
    }
  },
  components: {

  },
  ready(){
  	
  },
  methods: {

      
  }
}
</script>

<style>
  ul{
    width:100%;
  }
  ul>li{
    float:left;
    width:100%;
  }
  img{
    width:100%;
    height:100%;
  }

</style>





