<template>

  <button class="get-started">Get started for free</button>

</template>

<script>
export default {
  name: 'GetStartedBtn'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';
  
  button{
    border: none;
    background-color: $primary-color;
    color: white;
    padding: 13px 30px;
    border-radius: 7px;
    font-weight: 900;
    font-size: 14px;
  }
</style>