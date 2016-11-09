<template>
  <div class="container">
        <title-page :title='title' target='homemy.html' mode='dialog'>          
        </title-page>
     
        <diashenti>
        </diashenti>
</template>

<script>

import Lib from 'assets/Lib.js'
import titlePage from'components/titlePage'
import diashenti from 'components/diashenti'
module.exports = {
    components:{
        titlePage,diashenti,
    },
  data: function () {
    return {
    
    }
  },
  ready(){
    
  },
  methods:{
    
  },
  props:['title']
}
</script>


<style scoped>
.diacontent{
  width: 100%;
}
</style>
