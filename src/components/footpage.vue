<template>
  <div class="footbody">
  <ul class="clearfix">
     <li v-for=' info in aboutimgs'>
       <a :href='info.target' >
       <img :src="info.path" :class='info.name'>
       </a>
       <span>{{info.texttitle}}</span>
     </li>

  </ul>
  </div>
</template>

<script>

import Lib from 'assets/Lib.js'

module.exports = {
    components:{
        
    },
  data: function () {
    return {
      aboutimgs:[{path:require("../assets/img/images/04_22.png"),target:'#',texttitle:'首页',name:'first'

      },{path:require("../assets/img/images/04_01_24.png"),target:'#',texttitle:'询问',name:'second'

      },{path:require("../assets/img/images/04_26.png"),target:'dynatic.html',texttitle:'提吧',name:'third'

      },{path:require("../assets/img/images/04_28.png"),target:'#',texttitle:'我的',name:'forth'

      }]
    }
  },
  ready(){ 
    function find(name){
      return document.getElementsByClassName(name)[0];
    }
    console.log('selected:'+this.selected);
    if(this.selected=='1'){
            console.log('selected:'+this.selected);
            var img=find('first');
            img['src']=require("../assets/img/images/04_01_22.png");

            //console.log(img);

    }
    else if(this.selected=='2'){
            var img=find('second');
            img['src']=require("../assets/img/images/04_07.png");
    }
    else if(this.selected=='3'){
      var img=find('third');
            img['src']=require("../assets/img/images/04_01_26.png");
    }
    else{
            var img=find('forth')
            img['src']=require("../assets/img/images/04_01_28.png");
    }
    
  },
  methods:{
    
  },
  props:['selected']
}
</script>


<style scoped>
.footbody{
  width: 100%;
  height: 3.2rem;
  background-color: #f7f7f7;
  position:fixed;
  bottom:0px;
}
a{
  display: block;
  height: 1.5rem;


}
a img{width: 1.2em;
}
li{
  float:left;
text-align: center;
  width: 25%;

}
li span{font-size: 0.8rem;}
</style>
