<template>

  <main>
    <div class="hero pt-5 text-center">
      <div class="container mb-container">
        <h2>Learn At Your Own Pace!</h2>
        <p>Get teamed up with people of the same will.</p>
        <GetStartedBtn />
      </div>
      <div class="jumbo-images position-relative pt-5">
        <img class="hero-left-person" src="../assets/img/home-6-hero-left-person.png" alt="statistics">
        <div class="hero-big-image-container position-relative">
          <img class="hero-big-image" src="../assets/img/home-6-hero-poster-final.jpg" alt="statistics">
          <img class="youtube-icon" src="../assets/img/icon-youtube-play.png" alt="statistics">
        </div>
        <img class="hero-right-person" src="../assets/img/home-6-hero-right-person.png" alt="statistics">
      </div>
    </div>

    <div class="achievement">
      <div class="container mb-container text-center">
        <h3>Let passion and determination be the guide along the way and develop at your own pace that's comfortable.</h3>
        <div class="quote-author text-center">
          <h6>FANNIE MORENO</h6>
          <span>/Founder & CEO</span>
        </div>

        <div class="statistics d-flex justify-content-between">
          <div>
            <h3>1.926</h3>
            <span>FINISHED SESSIONS</span>
          </div>
          <div>
            <h3>3.092+</h3>
            <span>ENROLLED LEARNERS</span>
          </div>
          <div>
            <h3>200</h3>
            <span>ONLINE ISTRUCTORS</span>
          </div>
          <div>
            <h3>100%</h3>
            <span>SATISFACTION RATE</span>
          </div>
        </div>
      </div>
    </div>

    <div class="services">
      <div class="container mb-container d-flex">

        <div class="mb-columns d-flex">

          <div class="mb-column mb-column-1">
            <div class="mb-service-card">
              <div class="card-description">
               <h5>Graphic Design</h5>
               <p>Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.</p>
              </div>
              <div class="card-image card-image-1"></div>
           </div>
  
            <div class="mb-service-card">
              <div class="card-image card-image-3"></div>
              <div class="card-description">
               <h5>Idea Discussion</h5>
               <p>Get teamed up with the specialists who work and teach coding for years at famous universities</p>
              </div>
            </div>
         </div>
  
         <div class="mb-column mb-column-2">
            <div class="mb-service-card">
              <div class="card-description">
               <h5>Business Administration</h5>
               <p>Leaners are encouraged to study the mechanism and structure of suystem administation.</p>
              </div>
              <div class="card-image card-image-2"></div>
           </div>
  
            <div class="mb-service-card">
              <div class="card-image card-image-4 m-2"></div>
              <div class="card-description">
               <h5>Web Development</h5>
               <p>Learn to start building a webpage from scatch. you decide your own pace, course and speed.</p>
              </div>
            </div>
         </div>

        </div>

        <div class="premise">
          <p>TOGETHER WE CAN CREATE</p>
          <h1>Services We <span>Can Provide</span> For My Clients.</h1>
          <p><i class="fa-solid fa-check"></i> Select & customize courses to your preferences</p>
          <p><i class="fa-solid fa-check"></i> Change the tutor and make arrangements</p>
          <p><i class="fa-solid fa-check"></i> Partecipate in events to join others</p>
          <p><i class="fa-solid fa-check"></i> Get the desired certificate delivered at house</p>

          <GetStartedBtn />
        </div>

      </div>
    </div>

  </main>
  
</template>

<script>
  import GetStartedBtn from './GetStartedBtn.vue';

  export default {
    name: "MainComp",
    components: { GetStartedBtn }
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  .hero{
    background-color: #1f2154;
    color: white;
    max-height: 570px;
    margin-bottom: 100px;
    .jumbo-images{
      overflow: hidden;
      height: 515px;
      .hero-left-person{
        position: absolute;
        bottom: 0;
        left: 220px;
      }
      .hero-big-image-container{
        width: 800px;
        margin: 0 auto;
        .hero-big-image{
          border: 20px solid white;
          border-radius: 15px;
          box-shadow: 1px 5px 8px rgba($color: #000000, $alpha: 0.1);
        }
        .youtube-icon{
          position: absolute;
          top: 50%;
          left: 50%;
          transform: translate(-50%, -50%);
        }
      }
      .hero-right-person{
        position: absolute;
        bottom: -165px;
        right: 340px;
      }
    }
  }

  .achievement{
    margin-bottom: 100px;
    .mb-container{
      padding-top: 150px;
      h3{
        max-width: 550px;
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
      h3{
        color: $primary-color;
        font-weight: 900;
      }
      span{
        font-size: 13px;
      }
    }
  }

  .services{
    .mb-column{
      width: 250px;
      margin-right: 25px;
      .mb-service-card{
        margin-bottom: 25px;
        border: 1px solid black;
        .card-description{
          padding: 5px 14px;
          padding-top: 25px;
          p{
            font-size: 15px;
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
    }
    .mb-column-2{
      margin-top: 50px;
    }
    .premise{
      width: 400px;
      padding-top: 150px;
      margin-left: 100px;
      h1{
        margin-bottom: 40px;
      }
      span{
        color: $primary-color;
      }
      .fa-check{
        margin-right: 10px;
        color: $primary-color;
      }
    }
  }
</style>