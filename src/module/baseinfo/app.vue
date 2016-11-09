<template>
<div class="container">
<title-page :title='msg' target='homemy.html'></title-page>
 <div class='headimg'>
          <div  class="circle">
            <img src="../../assets/601.png">
          </div>
  </div>
 <ul>
   <li v-for='date in dates' class="clearfix">
     <span class="left">{{date.left}}</span>
     <span class="right">{{date.right}}</span>
   </li>

 </ul>

</div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'

export default {
  data() {
    return {
      dates:[
      {left:'昵称',right:'木有'},
      {left:'手机号码',right:'17768368136'},
      {left:'性别',right:'女'},
      {left:'生日',right:'1995-01-01'},
      {left:'所在地',right:'江苏无锡'},

    ],
    msg:'基本信息'
  }
},
  components:{
titlePage
  },
  ready(){
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>
.container{
  width: 100%;height: 100%;font-family: '微软雅黑';
}
.homemy{
  width: 100%;height: 100%;
}
.circle{width:3.5rem;height: 3.5rem;border:2px solid white;
  position:absolute;margin:auto;
top:0;left: 0;bottom: 0;right: 0;
border-radius: 100%;}
.circle{overflow: hidden;}
.circle img{width: 100%;height: 100%;

}
.headimg{width:100%;height: 3.5rem;
       
         position: relative;
         overflow: hidden;}
         .left{float: left;color: #272727;}
         .right{float: right;color: #1e2746;}
         ul{width: 80%;margin-left: 10%;
       }
       ul li{
        border-bottom: 1px solid #1e2746;
        font-size: 0.75rem;
        height: 2.25rem;
       }
       li span{height: 100%;line-height: 3rem;}
</style>





