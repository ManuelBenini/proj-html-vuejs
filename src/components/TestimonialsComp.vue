<template>

  <div class="testimonials">
    <div class="mb-container">

      <div class="text-center">
        <SectionTitle firstText="Why People Talk About" coloredText="MaxCoach" secondText="?" />
      </div>


      <div class="content d-flex position-relative">

        <div class="image-container position-relative">
          <img src="../assets/img/testimonial-avata-02.jpg" alt="testimonial-image">
        </div>

        <img class="shape" src="../assets/img/maxcoach-shape-05.png" alt="testimonial-image">
        <div class="circles">
          <div class="brown-fill"></div>
          <div class="brown-fill brown-fill2"></div>
          <div class="brown-fill brown-fill3"></div>
        </div>

        <div class="description">
          <p>I am free to learn at my own pace, follow my own schedule and choose the subject I like. Great study portal for people like me.</p>
          <QuoteAuthor author="MINA HOLLACE" role="Freelancer" />
        </div>


      </div>

      <div class="society-partners">

        <ul class="d-flex align-items-baseline">
          <li><a href="https://it.wikipedia.org/wiki/Acqua" target="_blank"><img src="../assets/img/client-logo-colored-01.png" alt="partners-logo"></a></li>
          <li><a href="https://www.adroll.com/" target="_blank"><img src="../assets/img/client-logo-colored-02.png" alt="partners-logo"></a></li>
          <li><a href="https://www.mozilla.org/it/firefox/" target="_blank"><img src="../assets/img/client-logo-colored-03.png" alt="partners-logo"></a></li>
          <li><a href="https://www.mobili-per-bambini.it/" target="_blank"><img src="../assets/img/client-logo-colored-04.png" alt="partners-logo"></a></li>
          <li><a href="https://bullfitfashion.com/it/" target="_blank"><img src="../assets/img/client-logo-colored-05.png" alt="partners-logo"></a></li>
          <li><a href="http://www.sixbasetech.com/" target="_blank"><img src="../assets/img/client-logo-colored-06.png" alt="partners-logo"></a></li>
        </ul>

      </div>

    </div>
  </div>
  
</template>

<script>
  import SectionTitle from './SectionTitle.vue';
  import QuoteAuthor from './QuoteAuthor.vue';

  export default {
    name: 'TestimonialsComp',
    components: {SectionTitle, QuoteAuthor}
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .testimonials{
    padding: 80px 0;
    .content{
      margin-top: 100px;
      padding: 0 100px;
      .image-container{
        width: 200px;
        height: 200%;
        border-radius: 50%;
        overflow: hidden;
        img{
          position: relative;
          z-index: 2;
          width: 100%;
          height: 100%;
        }
      }
      .shape{
        z-index: 1;
        position: absolute;
        bottom: 53px;
        left: 151px;
        width: 13%;
      }
      .circles{
        & *{
          position: absolute;
          border-radius: 50%;
          border: 1px solid
        }
        .brown-fill{
          z-index: 1;
          top: -15px;
          left: 120px;
          width: 70px;
          height: 70px;
          background-color: #d2a98e;
          border: none;
        }
        .brown-fill2{
          top: 5px;
          left: 190px;
        }
        .brown-fill3{
          top: 50px;
          left: 99px;
        }
      }
      .description{
        margin-left: 110px;
        width: 570px;
        font-size: 26px;
        margin-bottom: 70px;
      }
    }
    .society-partners{
      padding: 0 40px;
      li{
        margin-right: 70px;
        a{
          img{
            object-fit: cover;
          }
        }
      }
    }
  }

</style>