<template>
  <HeaderComponent />
  <JumboComponent />
  <MainComponent />
  <FooterComponentTop />
  <FooterComponent />
  <FooterComponentBottom />
   
</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue';
  import JumboComponent from './components/JumboComponent.vue';
  import MainComponent from './components/MainComponent.vue';
  import FooterComponent from './components/FooterComponent.vue';
  import FooterComponentTop from './components/FooterComponentTop.vue';
  import FooterComponentBottom from './components/FooterComponentBottom.vue';
  
  export default {
    name:'App',
    components:{
      HeaderComponent,
      MainComponent,
      FooterComponent,
      FooterComponentTop,
      FooterComponentBottom,
    }
  }
</script>

<style lang="scss" scoped>

</style>

