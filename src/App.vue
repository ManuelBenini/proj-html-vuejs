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

</style>
