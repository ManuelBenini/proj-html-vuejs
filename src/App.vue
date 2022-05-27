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
  @import '~@fontsource/poppins/index.css';
  @import '~@fontsource/poppins/600.css';
  @import '~@fontsource/poppins/700.css';
  @import '~@fontsource/poppins/800.css';
  @import '~@fontsource/poppins/900.css';

  body{
    font-family: "Poppins";
  }
  ul{
    list-style: none;
    margin: 0;
    padding: 0;
  }
  a{
    text-decoration: none;
  }
  .mb-container{
    max-width: 1210px;
  }

</style>
