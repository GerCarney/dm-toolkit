<template>
  <div id="app">
    <div class="content">
        <character/>
        <character/>
        <character/>
    </div>
    <div class="bottom">
    <md-bottom-bar>
      <md-bottom-bar-item md-icon="create">Create</md-bottom-bar-item>
      <md-bottom-bar-item md-icon="error">Combat</md-bottom-bar-item>
    </md-bottom-bar>
    </div>

  </div>
</template>

<script>

import Vue from 'vue'
import VueMaterial from 'vue-material'
require('vue-material/dist/vue-material.css')

Vue.use(VueMaterial)
Vue.material.registerTheme('default', {
primary: 'blue',
accent: 'red',
warn: 'red',
background: 'white'
})



import Character from './components/Character'

export default {
  name: 'app',
  components: {
    Character
  },
  mounted(){
  }
}
</script>

<style>

#app * {
  box-sizing:border-box;
}

</style>

<style scoped lang="scss">

  #app{
    display:flex;
    flex-direction:column;
    flex-grow:1;
    flex:1;

    .content{
      flex-grow:1;
      flex:1;
    }

    .bottom{
      position:absolute;
      left:0;
      bottom:0;
      right:0;
    }
  }

</style>
