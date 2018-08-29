<template>
  <div class="hello">
  <el-button @click="visible = true">Button</el-button>
    <h1>-----user:::{{ msg }}</h1>

  </div>
</template>

<script>
export default  {
  name: 'USER',
  data  : function() {
    return {
      msg: "user name: hu"
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
