<template>
  <div class="title clearfix">
   <a :href='target'><img :src="imgpath"></a>
   <p>{{title}}</p>
</div>
</template>

<script>

import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data: function () {
    return {
      imgpath:require('assets/img/images/03_03_03.png')
    }
  },
  ready(){
    console.log(this.mode);
    if(this.mode=='dialog')
    {
      var div=document.querySelector('.title');
      div.style.backgroundColor='#2b8bc5';
      var a=document.querySelector('a');
      a.innerHTML='';
      a.style.backgroundPosition='-49px -302px';
      a.style.width='0.6rem'
      a.style.height='0.9rem'
      div.style.color='white';
      console.log(div)
   document.querySelector('p').style.color='white';
    }
    
  },
  methods:{

    
  },
  props:['title','target','mode']
}
</script>


<style scoped>

.title{
  width:90%;
height:2.2rem; 
padding-left: 10%;
padding-top: 1rem;

}
.title a{
float:left;
width:0.45rem;
height:0.8rem;
background-image: url('../assets/picnew.png');
background-position: 0 0;
}
.title a img{
  width:100%;
  height:100%;
}

.title p{
margin-left: 40%;
width:3.4rem;
height:1.6rem;

color:#005e94;
font-size:0.75rem;
font-family: '黑体';
}
</style>
