<template>
  <div id="app">



  <div>
      <el-button @click="startHacking">Start</el-button>
    </div>
  HHHHHHH::::
    <div>{{ message }}</div>
    <User></User>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Hi"/>
  </div>
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import User from './components/user.vue'
export default {
  name: 'app',

    methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  },
  data: function(){
    return {
      message: 'Hello Vue!'
    }
  },


     components: {
          HelloWorld,
          User
     }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
