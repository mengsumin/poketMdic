<template>
<div class="pic">
  <img src="../assets/yao_03.png">
</div>
<div class="sedai"></div>
  <ul class="list">
  <li>
    <p>【药瓶名称】</p>
     <p>商品名称：{{mes.tradetitle}}</p>
     <p>通用名称：{{mes.commontitle}}</p>
  </li>
  <li>
      <p>【成分】</p>
      <p>{{mes.composition}}</p>
  </li>
  <li>
      <p>【功能主治】</p>
      <p>{{mes.functions}}</p>

  </li>
  <li>
    <p>【不良反应】</p>
     <p>{{mes.reaction}}</p>
  </li>
  <li>
    <p>【禁忌】</p>
    <p>{{mes.not}}</p>
  </li>
</ul>
</template>

<script>

import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data:function () {
    return {}
     
  },
  ready(){
    
  },
  methods:{
    
  },
  props:['mes']
}
</script>


<style scoped>
.sedai{
  height: 1rem;width: 100%;background-color: #f5f5f5;
}
.pic{

width: 100%;
height: 6rem;
padding: 1rem;
background-color: white;
text-align: center;
line-height: 6rem;
}
.pic img{
  width: 70%;height: 70%;


}
ul {
  width: 90%;
  margin-left: 5%;
  font-family: '微软雅黑';
}
li{
  margin-bottom: 0.7rem;
}
p{
  font-size: 0.75rem;
 
    margin-bottom: 0.5rem;
  
}
</style>
