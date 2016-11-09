<template>
<div class="medicinfo">
<title-page title='药品详情' mode='dialog'></title-page>
</div>
<medicinfo :mes='datas'></medicinfo>

</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from 'components/titlePage'
import medicinfo from 'components/medicinfo'

export default {
  data() {
    return {
      datas:{
        tradetitle:'江中',
        commontitle:'健胃消食片',
        composition:'太子参，陈皮，闪耀，麦芽，山楂，辅料为蔗糖，糊精，硬脂酸镁',
        functions:'健胃消食。用于脾胃虚弱所致的积食，症见不思饮食，暖腐酸臭。脘腹胀满。消化不良见上述证候者。',
        reaction:'尚不明确',
        not:'尚不明确'
      }
    
    }
  },
  components: {
titlePage,medicinfo
  },
  ready(){
  	
  },
  methods: {

      
  }
}
</script>

<style scoped>
.medicinfo{
  width: 100%;
}


</style>





