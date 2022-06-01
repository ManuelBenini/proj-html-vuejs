<template>

  <div class="learn-categories position-relative">

    <div class="circles">
      <div class="green"></div>
      <div class="orange-fill"></div>
      <div class="green-fill"></div>
    </div>

    <div class="mb-container">

      <div class="text-center">
        <SectionTitle title="WANNA TRANSFORM YOUR LIFE?" firstText="Glad to" coloredText="Help You" secondText="Learn" />
      </div>

      <div class="content">

        <div class="mb-cards-container d-flex">

          <LearnCategoryCard 
            icon="bi-flag" 
            title="Idea Discussion" 
            description="Get Teamed up with the specialists who work and teach coding for years at famous universities."
          />

          <LearnCategoryCard 
            icon="bi-gear" 
            title="Web Development" 
            description="Learn to start building a webpage from scratch. You decide your own pace, course and speed."
          />

          <LearnCategoryCard 
            icon="bi-life-preserver" 
            title="System Administration" 
            description="Learners are encouraged to study the mechanism and structure of system administration."
          />

          <LearnCategoryCard 
            icon="bi-display" 
            title="Graphic Design" 
            description="Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness."
          />

        </div>

        <div class="bottom-image">
          <img src="../assets/img/home-6-services-image.png" alt="">
        </div>

      </div>

    </div>
  </div>
  
</template>

<script>
  import SectionTitle from './SectionTitle.vue';
  import LearnCategoryCard from './BlogCard.vue';

  export default {
    name: 'TestimonialsComp',
    components: {SectionTitle, LearnCategoryCard}
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .learn-categories{
    padding-top: 70px;
    background: linear-gradient(white, $sections-color);
    .circles{
      & *{
        position: absolute;
        border-radius: 50%;
        border: 1px solid
      }
      .green{
        top: 510px;
        left: 480px;
        width: 50px;
        height: 50px;
        border: 5px solid #8fd6ca;
      }
      .orange-fill{
        bottom: 50px;
        left: 110px;
        width: 30px;
        height: 30px;
        background-color: #ff8265;
        border-color: #ff5000;
      }
      .green-fill{
        bottom: 400px;
        left: 1500px;
        width: 40px;
        height: 40px;
        background-color: #bce6df;
        border: none;
      }
    }
    .content{
      margin-top: 70px;
      .bottom-image{
        margin-top: 110px;
        img{
          width: 100%;
          height: 100%;
          transform: translate(0, 28px)
        };
      }
    }
  }

</style>