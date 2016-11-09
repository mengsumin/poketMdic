<template>
<div class='container'>
<title-page :title='msg' target='homemy.html'></title-page>
<doc-like v-for="doctor in doctors" :docinfo='doctor'><doc-like>

</div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'
import docLike from 'components/docLike'
export default {
  data() {
    return {
      msg:'关注',
      doctors:[
      {name:'朱正凯',vocation:'主治医师',position:'江苏省无锡市华东疗养院|内科',goodat:'糖尿病，冠心病，高血压',power:'1',num:0

      },
      {name:'胡飞',vocation:'主治医师',position:'江阴市中医院|骨科',goodat:'血管损伤，手外伤，骨折',power:'1',num:1

      },
      {name:'朱峰涛',vocation:'主治医师',position:'宜兴市人名医院|呼吸内科',goodat:'待完善',power:'14',num:2

      }
      ]

    }
  },
  components: {
      titlePage,docLike
  },
  ready(){
    
  },
  methods: {

      
  }
}
</script>

<style scoped>
.container{height: 100%;width: 100%;overflow: scroll;

}

</style>





