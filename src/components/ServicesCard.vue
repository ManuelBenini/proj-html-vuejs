<template>

  <div class="mb-service-card">
    <div v-if="inverse" :class="`card-image card-image-${imageNumber}`"></div>
    <div class="card-description">
      <h5>{{title}}</h5>
      <p>{{text}}</p>
    </div>
    <div v-if="!inverse" :class="`card-image card-image-${imageNumber}`"></div>
  </div>
  
</template>

<script>
export default {
  name: 'ServicesCard',
  props:{
    title: String,
    text: String,
    inverse: Boolean,
    imageNumber: String
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .mb-service-card{
    padding-top: 20px;
    background-color: white;
    margin-bottom: 25px;
    box-shadow: 1px 1px 15px rgba($color: #000000, $alpha: 0.1);
    .card-description{
      padding: 25px 7px 5px 14px;
      p{
        font-size: 15px;
        font-weight: 400;
      }
      h5{
        color: #1f2154;
      }
    }
    .card-image{
      height: 160px;
      background-repeat: no-repeat;
      background-size: contain;
    }
    .card-image-1{
      margin-left: 5px;
      background-image: url('../assets/img/home-6-service-image-01.png');
      background-position: left;
    }
    .card-image-2{
      background-image: url('../assets/img/home-6-service-image-02.png');
      background-position: center;
    }
    .card-image-3{
      background-image: url('../assets/img/home-6-service-image-03.png');
      background-position: left;
    }
    .card-image-4{
      background-image: url('../assets/img/home-6-service-image-04.png');
      background-position: center;
    }
  }

</style>