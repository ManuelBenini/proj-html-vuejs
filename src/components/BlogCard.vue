<template>

  <div class="mb-card">

    <div class="img-container">
      <img :src="isImageJpeg ? require(`../assets/img/${image}.jpeg`) : require(`../assets/img/${image}.jpg`)" alt="blog-image">
    </div>

    <div class="description mt-4">
      <h6><ColoredTextComp :text="artist" color="grey"/></h6>
      <h4>{{blogTitle}}</h4>
    </div>

    <div class="blog-statistics d-flex mt-4">
      <p><i class="fa-regular fa-calendar"></i>{{date}}</p>
      <p><i class="fa-regular fa-eye"></i>{{views}} views</p>
    </div>

  </div>

</template>

<script>
  import ColoredTextComp from './ColoredTextComp.vue';
  export default {
    name: "BlogCard",
    props: {
      image: String,
      isImageJpeg: Boolean,
      artist: String,
      blogTitle: String,
      date: String,
      views: String
    },
    components: {ColoredTextComp}
  }
</script>

<style lang="scss" scoped>

  .mb-card{
    width: calc(100% / 3 - 20px);
    margin-right: 20px;
    .img-container{
      img{
        width: 100%;
        border-radius: 5px;
      }
    }
    .blog-statistics{
      p{
        margin-right: 20px;
        color: grey;
        font-size: 14px;
      }
      i{
        margin-right: 8px;
      }
    }
  }

</style>