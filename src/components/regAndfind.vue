<template>
<div class="container">
<title-page :title='title' :target='target'></title-page>
 <label class="linktext clearfix"><span>手机号</span>
    <input type="" name="" placeholder="请输入手机号码">      
 </label>
 <label class="linktext clearfix"><span>验证码</span>
    <input type="" name="" placeholder="请输入验证码">      
 </label>
 <label class="linktext clearfix"><span>密码</span>
    <input type="" name="" placeholder="请输入密码">      
 </label>
 <button>提交</button>
</div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'
module.exports = {
	components:{
		titlePage
	},
  data: function () {
    return {
      target:'debark.html',
      msg: 'Hello moto! what`s up,yaoyao'
    }
  },
  ready(){
  	
  },
  methods:{
  	
  },
  props:['title']
  
}
</script>


<style scoped>
.container{
     font-family: '黑体';
     background-color: white;
}
input{
 float:right;
  border:0px;
  width:7.5rem;
  margin-left:1.24rem;
  position:relative;
  top:2.3rem;


}
label{
display:block;
 width:12.4rem;
  height:3.35rem;
    margin-left:2.675rem;
   border-bottom:0.1rem solid #999999;
   padding-left:0.85rem;
   font-size:0.75rem;
  
   line-height:5.35rem;
   color:#212650;
   outline: 0px;
   border:0px;
}
.linktext{
  display:block;
 
}
label span{
  width: 1.125rem;
}
button{
color:white;
  width:13rem;
  height:3.15rem;
  background-color:#005e94;
  border-radius:0.2rem;
  margin-left:2.8rem;
  border:0px;
  margin-top:4.15rem;
  font-size: 0.75rem;
  font-family: '黑体';
}
</style>
