<template>
<div class="dynatic">
  <div class="buttonmy clearfix">
      <span class="shehui">社区动态</span>
      <span class="my"> 我的动态</span>
  </div> 
  <p class="askinput clearfix">
    <input type="" name="" placeholder="你的问题" />
    <button>提交 </button>
    <div class="dymes">
       <question v-for='date in tigong' :mes='date'></question>
    </div>
   
  </p> 
</div>
<footpage selected='1'></footpage>

</template>

<script>

import Lib from 'assets/Lib.js'
import question from 'components/question'
import footpage from 'components/footpage'
export default {
  data() {
    return {
      tigong:[{title:'阿娇红枣和茯苓隔水炖，锅水炖干了，还可以吃吗？',name:'路人甲',answer:'可以的',time:'10 分钟前',text:'耳朵里面疼怎么办啊'},{title:'耳朵里面疼，好像被堵住了，不知道是不是有脓',name:'路人甲',answer:'可以的',time:'10 分钟前',text:'阿娇红枣和茯苓隔水炖，锅水炖干了，还可以吃吗？'}]
    }
  },
  components: {
question,footpage
  },
  ready(){
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>
.dynatic{
  width: 100%;
  height: 100%;
}
.buttonmy{
  width: 60%;
  height: 1.5rem;
  border: 1px solid #2e8acd;
  font-size: 0.8rem;
  line-height: 1.5rem;text-align: center;
  border-radius: 0.5rem;margin-left: 20%;overflow: hidden;
   margin-top: 1rem;
   margin-bottom: 0.7rem;
}
.buttonmy span{
  display: block;float: left;
  width: 50%;height: 100%;text-align: center;line-height: 1.5rem;

}
.shehui{
  background-color: #2e8acd;color: white;
}
.my{color: #2e8acd;}
.askinput{
  display: block;
  width: 80%;height: 1.5rem;
  margin-left: 10%;
  border: 1px solid #272451;
  border-bottom: 0px;



}
.dymes{
  width: 100%;margin-top: 1rem;
}
.askinput input{
  display: block;
 width: 80%;
  height: 1.49rem;
  border: 0px;outline: null;float: left;
  position: relative;top:;
}
.askinput button{width: 20%;
    background-color: #2e8acd;color: white;
height: 100%;
border: 0px;outline: null;display: block;float: right;}

</style>





