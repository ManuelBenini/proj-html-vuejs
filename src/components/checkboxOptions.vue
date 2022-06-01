<template>

  <div>
    <p><i class="fa-solid fa-check"></i> {{text}}</p>
  </div>
  
</template>

<script>
export default {
  name: 'A_Statistic',
  props:{
    text: String
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .fa-check{
    margin-right: 10px;
    color: $primary-color;
  }

</style>