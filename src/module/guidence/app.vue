<template>

<ul>
      <li >  
      <img :src='paths[0]'>
      </img>
      </li>

      <li >  
      <img :src='paths[1]'>
      </img>
      </li>
</ul>

</template>


<script>

import Lib from 'assets/Lib.js'


export default {
  data() {
    return {
    paths:[require('../../assets/images/02_01.jpg'),require('../../assets/images/02_02.jpg')]

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

<style scoped>
img{width:100%;height:100%;}
body{
  overflow:hidden;
}
li{
  float:left;
}

</style>





