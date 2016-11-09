<template>
  <div class='diames clearfix'>
    <div class="headimg">
      <img src="../assets/dochead.png" alt="">
    </div>
    <div class='message'>{{mes.xiaoxi}}
     <div class="icon"></div>
    </div>
  </div>
</template>

<script>
 
import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data: function () {
    return {
      
    }
  },
  ready(){
    
  },
  methods:{
    
  },
  props:['mes']
}
</script>


<style scoped>
.headimg{width: 4rem;height: 4rem;float: right;
  border:1px solid #e5e5e5;
  border-radius: 50%;overflow: hidden;
background-color: #fafafa;border: 2px solid #f4f4f4;}

.headimg img{width: 100%;height: 100%;}
.message{float: right;
color: white;
background-color: #2b8bc5;
line-height: 3rem;
height: 3rem;
text-align: center;
font-size: 0.8rem;
margin-top: 1rem;
border-radius: 0.2rem;
margin-right: 1rem;
position: relative;
padding: 0.1rem;
}
.icon{
  background-image: url('../assets/sanjiao.png');position: absolute;left: 99%;
  width: 1rem;height: 75%;
  top:0px;
  background-repeat: no-repeat;
}
</style>
