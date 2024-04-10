<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />

  <!--  non sono riuscita a finire la prima parte andrò avanti più tardi o domani  -->
   
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterComponent from './components/FooterComponent.vue';
  export default {
    name:'App',
    components:{
      HeaderComponent,
      MainComponent,
      FooterComponent
    }
    
  }
</script>

<style lang="scss" scoped>

</style>

