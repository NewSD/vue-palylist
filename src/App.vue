<template>
  <div id="app">
    <app-header v-bind:title="title"></app-header>
    <users v-bind:users="users"></users>
    <users v-bind:users="users"></users>
    <app-footer v-bind:title="title"></app-footer>
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld'
  import Users from './components/Users'
  import Header from './components/Header'
  import Footer from './components/Footer'

  export default {
    name: 'App',
    data() {
      return {
        // title: "这是我的第一个Vue脚手架项目"
        users: [
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
          {name:"Herry",position:"Web开发",show:false},
        ],
        title:"传递的是一个值,number string boolean"
      }
    },
    components: {
      HelloWorld,
      "users": Users,
      "app-header": Header,
      "app-footer": Footer
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

  h1 {
    color: purple;
  }
</style>
