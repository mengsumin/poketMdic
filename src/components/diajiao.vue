<template>
  <div class="diafoot clearfix">
    <i  class="record"></i>
    <input v-on:keyup.enter='notify' type="text">
    <i class='more'></i>
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
    notify:function(evevt){
      let o ={}
      o.xiaoxi=event.currentTarget.value;
      console.log(this.msg);
     this.msg.push(o);
     var input=document.querySelector('input');
     input.value='';
    }
           
  },
  props:{msg:Array}
}
</script>


<style scoped>
 .diafoot{
  position: relative;
  width: 80%;
  position: fixed;
  bottom: 0px;
  padding-left: 10%;padding-right: 10%;
  background-color: #f1f1f1;
 }
 input{
  height: 1.4rem;
  margin-left: 1.2rem;
  border: 0px;
  outline: none;
 }
 i{

  display: block;
  width: 1.73rem;height: 1.72rem;
  background-image: url('../assets/picnew.png');
 }
 .record{float: left;background-position: -314px -483px;
  float: left;
 }
 .more{float: right;
background-position:-313px -427px;
 }
</style>
