<template>

  <div>
    <h3>{{title}}</h3>
    <span>{{text}}</span>
  </div>
  
</template>

<script>
export default {
  name: 'A_Statistic',
  props:{
    title: String,
    text: String
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  h3{
    color: $primary-color;
    font-weight: bold;
    font-size: 33px;
  }
  span{
    font-size: 14px;
    font-family: 'atma';
  }

</style>