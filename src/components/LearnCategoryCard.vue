<template>

  <div class="mb-card">

    <div class="icon-container">
      <i :class="`bi ${icon}`"></i>
    </div>

    <div class="description">
      <h5>{{title}}</h5>
      <p>{{description}}</p>
    </div>

  </div>

</template>

<script>
export default {
  name: "LearnCategoryCard",
  props: {
    icon: String,
    title: String,
    description: String
  },
}
</script>

<style lang="scss" scoped>

  .mb-card{
    width: calc(100% / 4 - 20px);
    margin-right: 20px;
    .icon-container{
      font-size: 60px;
    }
    .description{
      p{
        font-size: 14px;
      }
    }
  }

</style>