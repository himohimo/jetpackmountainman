<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <page-container />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import PageContainer from '@/components/PageContainer.vue'

export default {
  name: 'app',
  components: {
    PageContainer
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  height: 100vh;
  width: 100vw;
  font-family: 'Open Sans', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #262626;
  color: #ccc;
}
</style>
