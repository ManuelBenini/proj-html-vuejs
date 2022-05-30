<template>

  <div>
    <HeaderComp />
    <MainComp />
    <FooterComp />

  </div>

</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp
}
}
</script>

<style lang="scss">
  @import '~bootstrap/scss/bootstrap.scss';
  @import '~@fortawesome/fontawesome-free/css/all.min.css';
  @import '~@fontsource/manjari/index.css';
  @import '~@fontsource/manjari/100.css';
  @import '~@fontsource/manjari/700.css';
  @import './assets/style/variables';

  @font-face { font-family: Gilroy; font-weight: 400; src: url('./assets/Gilroy-font/Gilroy-Light.otf'); } 
  @font-face { font-family: Gilroy; font-weight: bold; src: url('./assets/Gilroy-font/Gilroy-ExtraBold.otf');}

  body{
    font-family: $primary-font;
    font-weight: bold;
  }
  h1,h2,h3,h4,h5,h6{
    font-weight: bold;
  }
  p{
    font-weight: 400;
  }
  ul{
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .section-title{
    font-weight: 400;
  }
  a{
    text-decoration: none;
  }
  .mb-container{
    max-width: 1040px;
    margin: 0 auto;
  }

</style>
