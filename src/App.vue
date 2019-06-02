<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <!--<HelloWorld/>-->
    <h1>{{title}}</h1>
    <users></users>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import Users from './components/Users'
export default {
  name: 'App',
  data(){
    return{
      title:"这是我的第一个Vue脚手架项目"
    }
  },
  components: {
    HelloWorld,
    "users":Users
  }
}
</script>

<style scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1{
  color: purple;
}
</style>
