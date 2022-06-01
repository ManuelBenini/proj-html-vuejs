<template>

  <div>
    <h6>{{author}}</h6>
    <span>/ {{role}}</span>
  </div>

</template>

<script>
export default {
  name: "QuoteAuthor",
  props: {
    author: String,
    role: String
  },
}
</script>

<style lang="scss" scoped>

  h6{
    font-family: 'atma';
    margin-top: 40px;
    margin-bottom: 0;
  }
  span{
    color: grey;
    font-size: 14px;
  } 

</style>