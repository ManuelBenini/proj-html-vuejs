<template>
  
  <span>
    <span v-if="color !== undefined" :style="`color: ${color};`">{{text}}</span>

    <span v-else class="primary">{{text}}</span>
  
  </span>

</template>

<script>
export default {
  name: 'ColoredTextComp',
  props:{
    text: String,
    color: String
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';  

  .primary{
    color: $primary-color;
  }

</style>