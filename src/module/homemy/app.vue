<template>
<div class="homemy">
    <div class='headimg'>
          <img src="../../assets/6.png">
           <div class='bgcloth'>
          </div>
          <a href="baseinfo.html">
          <div  class="circle">
            <img src="../../assets/601.png">
          </div>
          </a>
    </div>

  <ul class="titledir">
    <li v-for='date in dirs' class="clearfix">
    <a :href='date.linkto'>
      <i clas='i-left':style='{backgroundPosition:date.pos}' >
      </i>
      <span>{{date.text}}</span>
      <i class='i-right'>
      </i>
      </a>
 
    </li>
  </ul>
    <foot-page :selected='msg'>
    <foot-page>

</div>

</template>

<script>

import Lib from 'assets/Lib.js'
import footPage from 'components/footpage'

export default {
  data() {
    return {
      msg:'4',
      dirs:[{text:'关 注', pos:'-319px -540px',linkto:'certain.html'

      },{text:'消息中心',pos:'-319px -592px',linkto:'infolist.html'

      },{text:'意见反馈',pos:'-319px -641px',linkto:'retroaction.html'

      },{text:'系统设置',pos:'-319px -690px',linkto:'config.html'

      },{text:'分 享',pos:'-262px -689px',linkto:'share.html'

      }]

    }
  },
  components: {
      footPage
  },
  ready(){
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>

ul{ 
  margin-left: 7%;
 width:86%;
}
i{
  display: block;
  float:left;
  background-image:url('../../assets/picnew.png');
  width: 1.5rem;height: 1.5rem;
  position: relative;
  top:-0.2rem;
background-repeat: no-repeat;

}
.i-left{float:left;}
.i-right{
  float:right;
    background-position: -258px -579px;
}
li{
  width:100%;
  border-top: solid 1px  #e4e4e4;
  height: 1.2rem;
  padding-top:0.8rem;
  position: relative;
  line-height: 100%;
}
.homemy{
  width: 100%;height: 100%;
}
span{
  padding-left: 10%;
  font-size:0.75rem;
  color:#333954;
  word-spacing: 1rem;

}
.headimg{width:100%;height: 25%;
       
         position: relative;
         overflow: hidden;}
.headimg>img{width: 110%;height: 110%;

       }
.bgcloth{width: 100%;height: 100%;background-color: black;position: absolute;opacity: 0.3;top:0rem;}
.circle{width:3.5rem;height: 3.5rem;border:2px solid white;
  position:absolute;margin:auto;
top:0;left: 0;bottom: 0;right: 0;
border-radius: 100%;}
.circle{overflow: hidden;}
.circle img{width: 100%;height: 100%;

}
</style>





