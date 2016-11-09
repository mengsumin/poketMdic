<template>
  <div class="container clearfix">
    <div class="left">
    <img src="../assets/dochead.png">
    </div>
    <div class="right">
      <p><span class="name">{{docinfo.name}}</span>  <span>{{docinfo.vocation}}</span></p>
      <p>{{docinfo.position}}</p>
      <p>擅长:{{docinfo.goodat}}</p>
       <ul class="clearfix">
         <li v-for='date in dates'>
          <a href="">{{date}}</a>
         </li>
       </ul>
    </div>
  </div>
</template>

<script>

import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data: function () {
    return {dates:['图文','电话','视屏','私人']
    }
  },
  ready()
  {      console.log(this.docinfo.num)
    console.log(this.docinfo.power);
    var njum=this.docinfo.num;
    var style;
    function find(num)
    {
      var index;

      var ul=document.getElementsByTagName('ul')[njum];
      console.log(ul);
      for(var i=0;i<4;i++)
      {
        index=parseInt(num.charAt(i));
        console.log(index);
        if(index)
        {
          var el=ul.querySelector('li:nth-of-type('+(index)+')');
         
             style=el.style;
             // console.log(style);
             style.color='#2c2d5d';
             style.border='1px solid #2c2d5d';
             el=el.querySelector('a');
             el.style.color='#2c2d5d';
        }
      }
    }
     find(this.docinfo.power);
  },
    
  // },
  methods:{
    
  },
  props:['docinfo']
    
  
}
</script>


<style scoped>
.container{width: 100%;height: 7rem;position: relative;font-size: 0.75rem;
  border-bottom: 1px solid #9e9e9e;
}
.left{
  width: 5rem;height: 5rem;margin-top: 1rem;margin-left: 1rem;
  float: left;
}
.left img{width: 100%;height: 100%;}
.right{float: left;width: 10rem;margin-left: 1rem;

}
ul li{float: left;width: 1.8rem;height: 1.4rem;text-align: center;line-height: 1.4rem;margin-top: 0.5rem;margin-right: 0.2rem;
 border: 1px solid #9e9e9e;padding-right: 0.2rem;padding-left: 0.2rem;
}
li a{color:#9e9e9e;}
p{margin-top: 0.3rem;font-family: '微软雅黑'}
.name{
  color:#1e2341;font-size: 0.9rem;
}
</style>
