<template>
<div class="container">
<title-page :title='msg' :target='link'></title-page>
<div class="middle">
 <div class='startIcon'>
   <img :src='titlePath'/> 
   </div>
   <p class="icon">版本:V3.8.8</p>
</div>
      <p class="tel">客服电话：<span>4008088088</span></p>


      <div class='footcloth'></div>
      </div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'

export default {
  data() {
    return {
      msg:'关于',
       titlePath:require('../../assets/img/title.png'),
       link:'homemy.html'

    }
  },
  components: {
      titlePage
  },
  ady(){
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>
.container{
  width: 100%;height: 100%;overflow: hidden;
}

.startIcon{
       width:39.4%;
       height:22.8%;
       background-color:white;
       position:absolute;
       border-radius:30%;
       overflow:hidden;
       left:30%;
       top:20%;

}
.footcloth{
  width: 100%;background-color: #f5f5f5;
  height: 50%;
}
img{width: 100%;height: 100%}
.middle{
  padding-bottom: 2rem;
width: 100%;height: 30%;
background-color: #f5f5f5;
text-align: center;
}

.icon{
  display: block;
  color:#999999;
  font-size: 0.75rem;
  position: absolute;
  left: 0;right: 0px;top:42%;

}
.tel{display: block;height: 1.8rem;line-height: 1.8rem;text-align: center;font-size: 0.8rem;}
.tel span{color:#1b5e8a;font-size: 0.6rem;}
</style>





