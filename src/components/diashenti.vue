<template>
  <div class='diacontent'>
   <dia-text v-for='date in messages' :mes='date'></dia-text>
    <diajiao :msg="messages"></diajiao>
  </div>

</template>

<script>

import Lib from 'assets/Lib.js'
import diajiao from 'components/diajiao'
import diaText from'components/diaText'

module.exports = {
    components:{
        diajiao,diaText
    },
  data: function () {
    return {
      messages:[]
    }
  },
  ready(){
    
  },
  methods:{ 
    
  },
  props:{
    
  },
  // events:{
  //   'diafoot-msg':function(msg){
  //     this.messages.push(msg);
  //   }
  // }
}
</script>


<style scoped>
.diacontent{
  width: 100%;
  overflow: scroll;
}
</style>
