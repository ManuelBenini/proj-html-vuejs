<template>

  <button v-if="btnText != 'View all courses'">{{btnText}}</button>
  <button v-else>{{btnText}} <i class="fa-solid fa-arrow-right"></i></button>

</template>

<script>
export default {
  name: 'AccentBtnComp',
  props:{
    btnText: String
  }
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