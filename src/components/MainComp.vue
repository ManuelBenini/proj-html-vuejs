<template>

  <main>
    <div class="hero pt-5 text-center">

      <div class="elementor-shape elementor-shape-bottom" data-negative="false">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 100" preserveAspectRatio="none">
          <path class="elementor-shape-fill" opacity="0.33" d="M473,67.3c-203.9,88.3-263.1-34-320.3,0C66,119.1,0,59.7,0,59.7V0h1000v59.7 c0,0-62.1,26.1-94.9,29.3c-32.8,3.3-62.8-12.3-75.8-22.1C806,49.6,745.3,8.7,694.9,4.7S492.4,59,473,67.3z"></path>
          <path class="elementor-shape-fill" opacity="0.66" d="M734,67.3c-45.5,0-77.2-23.2-129.1-39.1c-28.6-8.7-150.3-10.1-254,39.1 s-91.7-34.4-149.2,0C115.7,118.3,0,39.8,0,39.8V0h1000v36.5c0,0-28.2-18.5-92.1-18.5C810.2,18.1,775.7,67.3,734,67.3z"></path>
          <path class="elementor-shape-fill" d="M766.1,28.9c-200-57.5-266,65.5-395.1,19.5C242,1.8,242,5.4,184.8,20.6C128,35.8,132.3,44.9,89.9,52.5C28.6,63.7,0,0,0,0 h1000c0,0-9.9,40.9-83.6,48.1S829.6,47,766.1,28.9z"></path>
        </svg>		
      </div>

      <div class="mb-container">
        <h2>Learn At Your Own Pace!</h2>
        <p class="mb-4">Get teamed up with people of the same will.</p>
        <AccentBtnComp class="whiteHoveredBtn" btnText="Get started for free" />
      </div>

      <div class="jumbo-images position-relative">
        <img class="left-person" src="../assets/img/home-6-hero-left-person.png" alt="left-image">

        <div class="big-image position-relative">
          <img class="hero-poster" src="../assets/img/home-6-hero-poster-final.jpg" alt="center-image">
          <img class="youtube" src="../assets/img/icon-youtube-play.png" alt="youtube-icon">
        </div>

        <img class="right-person" src="../assets/img/home-6-hero-right-person.png" alt="right-image">
        <div class="blank-div"></div>
      </div>

      <div class="side-menu">
        <div class="icon">
         <a href="#"><i class="bi bi-caret-right-square-fill"></i></a>  
        </div>

        <div class="icon">
         <a href="#"><i class="fa-regular fa-life-ring"></i></a> 
        </div>

        <div class="icon">
         <a href="#"><i class="fa-solid fa-book"></i></a>  
        </div>

        <div class="icon">
         <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>  
        </div>
      </div>
      
    </div>

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

    <div class="services">
      <div class="mb-container d-flex">

        <div class="mb-columns d-flex">

          <div class="mb-column mb-column-1">

            <ServicesCard 
              title="Graphic Design"
              text="Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness." 
              imageNumber="1"
              :inverse="false"
            />

            <ServicesCard 
              title="Idea Discussion"
              text="Get teamed up with the specialists who work and teach coding for years at famous universities" 
              imageNumber="3"
              :inverse="true"
            />

         </div>
  
         <div class="mb-column mb-column-2">

            <ServicesCard 
              title="Business Administration"
              text="Leaners are encouraged to study the mechanism and structure of system administation." 
              imageNumber="2"
              :inverse="false" 
            />

            <ServicesCard 
              title="Web Development"
              text="Learn to start building a webpage from scatch. you decide your own pace, course and speed." 
              imageNumber="4"
              :inverse="true"
            />

         </div>

        </div>

        <div class="services-to-create">

          <SectionTitle 
            title="TOGETHER WE CAN CREATE" 
            firstText="Services We" 
            coloredText="Can Provide" 
            secondText="For My Clients." 
          />

          <div class="options mt-5">
            <CheckboxOptions text="Select & customize courses to your preferences" />
            <CheckboxOptions text="Change the tutor and make arrangements" />
            <CheckboxOptions text="Partecipate in events to join others" />
            <CheckboxOptions text="Get the desired certificate delivered at house" />
          </div>

          <AccentBtnComp class="mt-3 blackHoveredBtn" btnText="Get started for free" />

        </div>

      </div>
    </div>

    <div class="courses">
      <div class="mb-container">

        <div class="text-center">
          <SectionTitle 
            title="CHOOSE A COURSE TO GET STARTED" 
            firstText="Latest Featured" 
            coloredText="Courses"
          />
        </div>

        <div class="mb-course-cards-container d-flex flex-wrap">

          <CourseCard 
            imageNumber="1" 
            coloredIntegerPrice="$40"
            coloredDecimalPrice=".00"
            courseDescription="Learning to Write as a Professional Author"
            lessons="20"
            students="50" 
          />

          <CourseCard 
            imageNumber="2" 
            coloredIntegerPrice="free"
            courseDescription="Customer-centric Info-Tech Strategies"
            lessons="24"
            students="769" 
          />

          <CourseCard 
            imageNumber="3" 
            coloredIntegerPrice="$19"
            coloredDecimalPrice=".00"
            courseDescription="Open Programming courses for Everyone: Python"
            lessons="17"
            students="62" 
          />

          <CourseCard 
            imageNumber="4" 
            coloredIntegerPrice="$26"
            coloredDecimalPrice=".00"
            courseDescription="Academic Listening and Note-taking"
            lessons="14"
            students="67" 
          />

          <CourseCard 
            imageNumber="5" 
            coloredIntegerPrice="$39"
            coloredDecimalPrice=".00"
            courseDescription="Master jQuery in a Short Period of Time"
            lessons="6"
            students="51" 
          />

          <CourseCard 
            imageNumber="6" 
            coloredIntegerPrice="$59"
            coloredDecimalPrice=".00"
            courseDescription="Introduction to Javascript for Beginners"
            lessons="14"
            students="76" 
          />

        </div>

        <div class="courses-btn text-center">
          <AccentBtnComp class="blackHoveredBtn" style="padding: 16px 65px;" btnText='View all courses' />
        </div>

      </div>
    </div>

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

    <div class="blogs">

      <div class="mb-container">

        <div class="text-center">
          <SectionTitle title="ENJOY READING ON MAXCOACH" firstText="Latest on" coloredText="Our Blogs" />
        </div>

        <div class="mb-cards-container mt-5 d-flex">

          <BlogCard 
            image="artist-blog-03-480x325" 
            :isImageJpeg="true"
            artist="ARTIST" 
            blogTitle="Brush Strokes Energize Trees In Paintings"
            date="May 15, 2020" views="688"
          />

          <BlogCard 
            image="artist-blog-01-480x325" 
            :isImageJpeg="false"
            artist="ARTIST" 
            blogTitle="Pocket-Sized Notebooks Hold Miniature Paintings"
            date="May 15, 2020" views="603"
          />

          <BlogCard 
            image="artist-blog-02-480x325" 
            :isImageJpeg="false"
            artist="ARTIST" 
            blogTitle="Connection Between Self-Portraits and Identity"
            date="May 15, 2020" views="397"
          />

        </div>

      </div>
    </div>

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

    <div class="call-to-action position-relative">

      <div class="circles">
        <div class="yellow-fill"></div>
        <div class="pink-fill"></div>
        <div class="azure-fill"></div>
      </div>

      <div class="mb-container text-center">

        <h5>Start today for getting <ColoredTextComp text="Online Certification"/></h5>
        <h2 class="mb-4">You can be your own guiding star with our help!</h2>
        <AccentBtnComp class="blackHoveredBtn" style="padding: 16px 65px;" btnText="Get started now"/>

      </div>

    </div>

  </main>
  
</template>

<script>
  import AccentBtnComp from './AccentBtnComp.vue';
  import ColoredTextComp from './ColoredTextComp.vue';
  import A_Statistic from './A_Statistic.vue';
  import ServicesCard from './ServicesCard.vue';
  import SectionTitle from './SectionTitle.vue';
  import CheckboxOptions from './CheckboxOptions.vue';
  import CourseCard from './CourseCard.vue';
  import QuoteAuthor from './QuoteAuthor.vue';
  import BlogCard from './BlogCard.vue';
  import LearnCategoryCard from './LearnCategoryCard.vue';


  export default {
    name: "MainComp",
    components: { AccentBtnComp, ColoredTextComp, A_Statistic, ServicesCard, SectionTitle, CheckboxOptions, CourseCard, QuoteAuthor, BlogCard, LearnCategoryCard }
  }
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';  

  .hero{
    position: relative;
    background-color: #1f2154;
    color: white;
    max-height: 646px;
    .whiteHoveredBtn{
      z-index: 99;
      position: relative;
      &:hover{
        background-color: white;
        color: $primary-color;
      }
    }
    .elementor-shape{
      transform: rotate(180deg);
      position: absolute;
      left: 0;
      bottom: -1px;
      line-height: 0;
      direction: ltr;
      overflow: hidden;
      z-index: 1;
      svg{
        height: 550px;
        display: block;
        width: calc(100% + 1.3px);
        position: relative;
        left: 50%;
        transform: translateX(-50%);
        overflow: hidden;
      }
      .elementor-shape-fill{
        fill: rgba(255, 255, 255, 0.03);
      }
    }
    .jumbo-images{
      text-align: center;
      height: 487px;
      margin: 0 auto;
      margin-top: 80px;
      overflow: hidden;
      z-index: 2;
      .left-person{
        position: absolute;
        z-index: 10;
        top: -32px;
        left: 210px;
      }
      .right-person{
        position: absolute;
        z-index: 9;
        bottom: -163px;
        right: 340px;
      }
      .blank-div{
        position: absolute;
        z-index: 60;
        bottom: -37px;
        right: 278px;
        background: white;
        height: 65px;
        width: 100px;
      }
      .big-image{
        .hero-poster{
          position: relative;
          z-index: 10;
          border: 20px solid white;
          border-radius: 20px;
          box-shadow: 1px 1px 15px rgba($color: #000000, $alpha: 0.1);
        }
        .youtube{
          position: absolute;
          top: 50%;
          left: 50%;
          z-index: 20;
          transform: translate(-50%, -50%);
          transition: all .3s linear;
          cursor: pointer;
          &:hover{
            top: 45%;
            left: 47%;
            transform: scale(1.5);
          }
        }
      }
    }
    .side-menu{
      border-top-left-radius: 5px;
      border-bottom-left-radius: 5px;
      padding-top: 7px;
      position: absolute;
      z-index: 9999;
      top: 70px;
      right: 0;
      width: 40px;
      background-color: white;
      a{
        color: black;
        &:hover{
          color: $primary-color;
        }
      }
      .icon{
        margin-bottom: 10px;
      }
    }
  }

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

  .services{
    .mb-container{
      padding-top: 130px;
      padding-bottom: 60px;
      background-image: url('../assets/img/background-pattern-grid-line.png');
      background-size: 331px 100px;
    }
    .mb-column{
      width: 250px;
      margin-right: 15px;
    }
    .mb-column-2{
      margin-top: 50px;
      margin-left: 10px;
    }
    .services-to-create{
      padding-top: 175px;
      margin-left: 52px;
      width: 380px;
      .blackHoveredBtn:hover{
        background-color: #3f3a64;
        color: white;
      }
    }
  }

  .courses{
    padding: 100px 0;
    background-color: $sections-color;
    .mb-container{
      .courses-btn{
        margin-top: 50px;
        .blackHoveredBtn:hover{
          background-color: #3f3a64;
          color: white;
        } 
      }
    }
  }

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

  .blogs{
    padding: 70px 0;
    background-color: $sections-color;
  }

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

  .call-to-action{
    padding: 100px 0;
    .blackHoveredBtn:hover{
      background-color: #3f3a64;
      color: white;
    } 
    .circles{
      & *{
        position: absolute;
        border-radius: 50%;
        border: 1px solid
      }
      .yellow-fill{
        top: 150px;
        left: 120px;
        width: 40px;
        height: 40px;
        background-color: #ebb860;
        border-color: #e7ab37;
      }
      .pink-fill{
        top: 5px;
        left: 1430px;
        width: 35px;
        height: 35px;
        background-color: #e88c98;
        border-color: #e37283;
      }
      .azure-fill{
        bottom: 175px;
        left: 1670px;
        width: 35px;
        height: 35px;
        background-color: #aab8f1;
        border-color: #9fafef;
      }
    }
  }
</style>