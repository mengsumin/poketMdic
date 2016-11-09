<template>
<div class="container">
<title-page :title='msg' :target='linkto'></title-page>
<p class='hen'></p>
<ul>
    <a href="about.html">
    <li style="border-top:none">关于 <i class='i'></i></li>


    </a>
    <li>    <a href="">检查更新</a></li>
    <li><a href="">退出</a></li>
</ul>

</div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'

export default {
  data() {
    return {
      msg:'设置',
      linkto:'homemy.html'

    }
  },
  components: {
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
  width: 100%;height: 100%;
}
.hen{
  display: block;height: 5%;background-color: #f5f5f5;
  position: relative;top:-1%;
}
ul{
  width: 100%;
}
  li{
    width: 80%;
    height: 1rem;
    font-size: 0.75rem;
    color:#202b3d;
    margin-left: 10%;
    padding-top: 0.5rem;padding-bottom: 0.5rem;
    border-top: 1px solid #e5e5e5;
  }
.i{width: 0.75rem;height: 0.75rem;float: right;
background-image: url('../../assets/picnew.png');
background-position: -273px -581px;

}
</style>





