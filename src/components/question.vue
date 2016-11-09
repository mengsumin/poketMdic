<template>
  <div class="question clearfix">
        <div class="bao">
        <i class="wenhao"> </i>
          <div class="baoText">
          <p class="til">{{mes.title}}</p>
          <p class="text">{{mes.text}}</p>
        
          <p class="time">{{mes.time}}</p>
          <i class="add"></i>

          <p class="answer"> <span id="name">{{mes.name}}:</span>
          {{mes.answer}}
          </p>
          <div>
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
#name{color: #1c213e;}
.answer{font-size: 0.8rem;color: #929292;}
.answer span{font-color:#1c213e;font-size: 0.8rem;}
.text{font-size: 0.8rem;color: #929292}
.til{color: #1c213e;font-size: 1rem;font-size: 0.8rem;width: 80%;}
.time{
  font-size: 0.8rem;color: #929292;
}
.question{
  width: 100%;
   height: 100%;
   border-bottom: 1px solid #e5e5e5;
   padding-bottom:1rem;
}
i{
  width: 25px;height: 25px;background-image: url('../assets/picnew.png');display: block;

}
.wenhao{
  background-position: -133px -415px;
  float: left;
  margin-right: 0.5rem;
  padding-bottom: 1rem;
}
.add{
  background-position: -133px -346px;margin-right: 100%;
    margin-left:  80%;

}
.bao{
  padding-left: 10%;
}
.baoText{
float: left;
width: 85%;
}
</style>
