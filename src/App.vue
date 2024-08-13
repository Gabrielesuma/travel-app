<template>
  <HeaderComponent/>
  <MainComponent/>
  <p>{{ message }}</p>
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  export default {
    name: 'App',
    components:{
      HeaderComponent,
      MainComponent
    },
    data(){
      return{
        message: 'ciao'
      }
    }
  }
</script>

<style lang="scss" scoped>
.red{
  color:red;
}
.blue{
  color: blue;
}
</style>