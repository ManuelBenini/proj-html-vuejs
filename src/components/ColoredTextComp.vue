<template>
  
  <span>{{text}}</span>

</template>

<script>
export default {
  name: 'ColoredTextComp',
  props:{
    text: String
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';  

  span{
    color: $primary-color;
  }

</style>