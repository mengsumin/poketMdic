<template>
 <div class='startIcon'>
   <img :src='titlePath'/>
</div>

<p class='copyright'>{{copyright}}</p>

</template>

<script>

import Lib from 'assets/Lib.js'


export default {
  data() {
    return {
    copyright:'Copyright@UlightCorporation',
    titlePath:require('../../assets/img/title.png')
   

    }
  },
  components: {

  },
  ready(){
  setTimeout(function(){
        location='guidence.html';
  },1500);
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>
.startIcon{
      margin-left:30.2%;
      margin-top:36%;
       width:39.4%;
       height:22.8%;
       background-color:white;
       position:absolute;
       border-radius:30%;
       overflow:hidden;

}
.copyright{
  color:white;
  padding-left:20%;
  font-size:1em;
  position:fixed;
  bottom:10%;
}
img{position:absolute;
width:100%;
height:100%;

}

</style>





