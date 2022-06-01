<template>

  <div class="mb-course-card d-flex">
    <div :class="`bg-image bg-image-${imageNumber}`"></div>

    <div class="course-description">
      <h4><ColoredTextComp :text="coloredIntegerPrice"/><ColoredTextComp class="course-decimal-price" :text="coloredDecimalPrice"/></h4>
      <h6>{{courseDescription}}</h6>
      <div class="course-statistics d-flex">
        <p><i class="fa-regular fa-file-lines"></i>{{lessons}} Lessons</p>
        <p><i class="fa-regular fa-user"></i>{{students}} Students</p>
      </div>
    </div>

  </div>

</template>

<script>
  import ColoredTextComp from './ColoredTextComp.vue';
  export default {
    name: "CourseCard",
    props: {
      imageNumber: String,
      coloredIntegerPrice: String,
      coloredDecimalPrice: String,
      courseDescription: String,
      lessons: String,
      students: String
    },
    components: { ColoredTextComp }
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .mb-course-card{
    width: calc(100% / 2 - 20px);
    margin-top: 40px;
    margin-right: 20px;
    padding: 20px 0;
    padding-left: 20px;
    cursor: pointer;
    &:hover{
      background-color: white;
    }
    &:hover h6{
      color: $primary-color;
    }
    .bg-image{
      height:150px;
      width: 150px;
      border-radius: 50%;
      margin-right: 20px;
      background-size: cover;
      background-position: center;
    }
    .bg-image-1{
      background-image: url('../assets/img/course-02-480x298.jpg');
    }
    .bg-image-2{
      background-image: url('../assets/img/stock-full-hd-03-480x298.jpg');
    }
    .bg-image-3{
      background-image: url('../assets/img/stock-full-hd-04-480x298.jpg');
    }
    .bg-image-4{
      background-image: url('../assets/img/stock-full-hd-06-480x298.jpg');
    }
    .bg-image-5{
      background-image: url('../assets/img/course-featured-image-01-480x298.jpg');
    }
    .bg-image-6{
      background-image: url('../assets/img/stock-full-hd-05-480x298.jpg');
    }
    h4{
      font-weight: 700;
    }
    h6{
      width: 290px;
      line-height: 30px;
      font-weight: 600;
      color: #342f5d;
    }
    .course-decimal-price{
      font-size: 18px;
    }
    .course-statistics{
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