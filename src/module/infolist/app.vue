<template>
<div class="container">
<title-page :title='msg' target='homemy.html'></title-page>
<doc-dialog v-for='date in dates' :docs='date'></doc-dialog>

</div>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'
import docDialog from 'components/docDialog'
export default {
  data() {
    return {
      msg:'消息中心',
      dates:[{
      name:'小一',mes:'好的',time:'20:23'
      },
      {name:'朱正凯',mes:'谢谢',time:'20::23'

      },
      {name:'官方消息',mes:'欢迎使用口袋医生',time:'18:00'}]

    }
  },
  components: {
      titlePage,docDialog
  },
  ready(){
    
  },
  methods: {

      
  }
}
</script>

<style scoped>
.container{
  width: 80%;margin-left: 10%;
}

</style>





