<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponentTop />
  <FooterComponent />

  <!--  non sono riuscita a finire la prima parte andrò avanti più tardi o domani  -->
   
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterComponent from './components/FooterComponent.vue';
  import FooterComponentTop from './components/FooterComponentTop.vue';
  
  export default {
    name:'App',
    components:{
      HeaderComponent,
      MainComponent,
      FooterComponent,
      FooterComponentTop,
    }
  }
</script>

<style lang="scss" scoped>

</style>

