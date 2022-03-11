<template>
  <div id="app">

    <StepForm/>
    <button @click="clickShowBtn()">Show Hello Worl</button>
  </div>
</template>

<script>
import StepForm from './components/StepForm.vue';

export default {
  name: 'App',
  components: {
    StepForm
  },
  data:function(){
    return {
      showHelloComp:false
    }
  },
  methods:{
    clickShowBtn(){
        this.showHelloComp = !this.showHelloComp;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
