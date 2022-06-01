<template>

  <div class="achievement position-relative">

    <div class="circles">
      <div class="green"></div>
      <div class="orange-fill"></div>
      <div class="yellow-fill"></div>
      <div class="purple-fill"></div>
      <div class="green-fill"></div>
      <div class="pink-fill"></div>
      <div class="azure-fill"></div>
      <div class="pink"></div>
    </div>

    <div class="mb-container text-center">

      <div class="description">
        <h3>Let passion and determination be the guide along the way and develop at your own pace that's comfortable.</h3>
        <div class="quote-author text-center">
          <QuoteAuthor author="FANNIE MORENO" role="Founder & CEO" />
        </div>

        <div class="statistics d-flex justify-content-between">

          <A_Statistic title="1.926"  text="FINISHED SESSIONS" />
          <A_Statistic title="3.092+"  text="ENROLLED LEARNERS" />
          <A_Statistic title="200"  text="ONLINE ISTRUCTORS" />
          <A_Statistic title="100%"  text="SATISFACTION RATE" />

        </div>

      </div>

    </div>

  </div>
  
</template>

<script>
  import A_Statistic from './A_Statistic.vue';
  import QuoteAuthor from './QuoteAuthor.vue';

  export default {
    name: 'AchievementComp',
    components: {A_Statistic, QuoteAuthor}
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .achievement{
    .circles{
      & *{
        position: absolute;
        border-radius: 50%;
        border: 1px solid
      }
      .green{
        top: 150px;
        left: 280px;
        width: 50px;
        height: 50px;
        border: 5px solid #8fd6ca;
      }
      .orange-fill{
        top: 350px;
        left: 310px;
        width: 30px;
        height: 30px;
        background-color: #ff8265;
        border-color: #ff5000;
      }
      .yellow-fill{
        top: 520px;
        left: 180px;
        width: 40px;
        height: 40px;
        background-color: #ebb860;
        border-color: #e7ab37;
      }
      .purple-fill{
        top: 190px;
        left: 830px;
        width: 20px;
        height: 20px;
        background-color: #bc71fe;
        border-color: #b75cfe;
      }
      .green-fill{
        top: 90px;
        left: 1570px;
        width: 40px;
        height: 40px;
        background-color: #bce6df;
        border: none;
      }
      .pink-fill{
        top: 275px;
        left: 1570px;
        width: 35px;
        height: 35px;
        background-color: #e88c98;
        border-color: #e37283;
      }
      .azure-fill{
        top: 425px;
        left: 1370px;
        width: 35px;
        height: 35px;
        background-color: #aab8f1;
        border-color: #9fafef;
      }
      .pink{
        top: 505px;
        left: 1560px;
        width: 55px;
        height: 55px;
        background-color: white;
        border: 8px solid #f6b9aa;
      }
    }
    .mb-container{
      background-image: url('../assets/img/background-pattern-grid-line.png');
      background-size: 331px 100px;
      padding: 0 08px;
      padding-top: 250px;
      h3{
        line-height: 40px;
        max-width: 590px;
        margin: 0 auto;
      }
      .quote-author{
        h6{
          margin-top: 40px;
        }
        span{
          color: grey;
          font-size: 14px;
        }
      }
    }
    .statistics{
      padding: 0 30px;
      padding-top: 100px;
      
    }
  }

</style>