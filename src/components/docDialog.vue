<template>
  <div class="docdialog clearfix">
       <div class="head">
            <img src="../assets/dochead.png">
        </div>
        <div class="text clearfix">
              <p class="name">{{docs.name}}</p>
              <p class="message">{{docs.mes}}</p>
              
        </div>
        <span class="time">{{docs.time}}</span>

  </div>
</template>

<script>

import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data: function () {
    return {
      msg: 'Hello moto! what`s up,yaoyao'
    }
  },
  ready(){
    
  },
  methods:{
    
  },
  props:['docs']
}
</script>


<style scoped>
.docdialog{
  width: 100%;
  font-family: '微软雅黑';

}
.head{width: 4rem;height: 4rem;float: left;
  border:1px solid #e5e5e5;
  border-radius: 50%;overflow: hidden;
background-color: #fafafa;border: 2px solid #f4f4f4;}
.text{float:left;;padding-left: 0.5rem;}
.head img{width: 100%;height: 100%;}
 span{float: right;padding-top: 1.15rem;}
 .time{font-size: 0.6rem;color: #9a9a9a;}
 .message{font-size: 0.7rem;color: #9a9a9a;}
 .text p.name{font-size: 0.8rem;color: #1f2755;}
.text p{padding-top: 1.15rem; }

</style>
