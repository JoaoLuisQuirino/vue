<template>
  <div id="app">

    <div v-if="showPage">
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div>
    <div v-else @click="toogleShowPage()">
      joao
    </div>
  </div>
</template>

<script>

export default {
  name: 'app',
  data: () => {
    return {
      showPage: false,
    }
  },
  components: {
    HelloWorld: () => import('./components/HelloWorld.vue')
  },
  methods:{
    toogleShowPage(){
      this.showPage = !showPage;
    }
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
