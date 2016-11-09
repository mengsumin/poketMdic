<template>
 <div class='container'>
 <div class='title clearfix'>
 <i><img :src='imgpath'></img></i>
    <p>登陆</p> 
    </div>
      <label>手机号
           <input placeholder='请输入手机号码'></input>
      </label>
      <label>密码&nbsp;
            <input placeholder='请输入密码'></input>  <i></i>
      </label>
<p class='linktext clearfix'> 
  <span class='linkleft'>
        <a href='regist.html' >快速注册</a>
  </span>  
  <span class='linkright'>
        <a href='findPassword.html'>忘记密码?</a>
  </span>
</p>

<button>登陆</button>

 </div>

</template>

<script>

import Lib from 'assets/Lib.js'


export default {
  data() {
    return {
     imgpath:require('assets/img/images/03_03_03.png')
    }
  },
  components: {

  },
  ready(){
  	
  },
  methods: {

      
  }
}
//height：1294
//height：750
</script>

<style scoped>
.container{
  width:100%;
  height:100%;
  background-color:white;
  font-family:'arial';
}
label{
  display:block;
}
button{
color:white;
  width:76.8%;
  height:6.5%;
  background-color:#005e94;
  border-radius:5%;
  margin-left:11.6%;
  border:0px;
  margin-bottom:39.4%;
}
.title{width:100%;
height:6.45rem; 
}
.title i{
display:inline-block;
float:left;
width:0.45rem;
height:0.8rem;
margin-left:2.25rem;
margin-top:3.4rem;
}
.title i img{
  width:100%;
  height:100%;
}

.title p{
display:inline-block;
float:left;
margin-top:3.4rem;
width:3.4rem;
height:1.6rem;
margin-left:6.25rem;
color:#005e94;
}
input{
 
  border:0px;
  width:7.5rem;
  margin-left:1rem;


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
}
.linktext{
  font-size:0.625rem;
  display:block;
  padding-top:1.4rem;
  padding-bottom:3.2rem;
 
}
.linktext a{
   color:#2a8bc3;
}
.linkleft{float:left;margin-left:2.3rem;}
.linkright{float:right;margin-right:2.3rem;}

</style>





