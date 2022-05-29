<template>

  <footer>
    <div class="container mb-container">
      <div class="lists-container d-flex">

        <ul class="flex-grow-1">
          <li class="mb-4"><h5>Address</h5></li>
          <li><p>382 NE 191st St # 87394 Miami, Fl 33179-3899</p></li>
          <li><p>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p></li>
          <li><p>support@maxcoach.com</p></li>
        </ul>

        <ul class="right-col">
          <li class="mb-4"><h5>Explore</h5></li>
          <li><a href="#"><p>Start here</p></a></li>
          <li><a href="#"><p>Blog</p></a></li>
          <li><a href="#"><p>About us</p></a></li>
        </ul>

        <ul class="right-col">
          <li class="story mb-4"><h5>Story</h5></li>
          <li><a href="#"><p>Success story</p></a></li>
          <li><a href="#"><p>Courses</p></a></li>
          <li><a href="#"><p>Contact us</p></a></li>
        </ul>

        <ul class="right-col">
          <li class="mb-4"><h5>Information</h5></li>
          <li><a href="#"><p>Membership</p></a></li>
          <li><a href="#"><p>Purchase guide</p></a></li>
          <li><a href="#"><p>Privacy policy</p></a></li>
          <li><a href="#"><p>Terms of services</p></a></li>
        </ul>
      </div>

      <div class="social">
        <ul class="d-flex">
          <li><a href="#"><i class="fa-brands fa-facebook-square"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
          <li><a href="#"><i class="fa-brands fa-linkedin"></i></a></li>
        </ul>
      </div>

      <div class="credits text-center">
        <span>&copy; 2020 Maxcoach. All Rights Reserved</span>
      </div>
    </div>

    <div class="return-up">
     <a href="#"><i class="bi bi-arrow-up"></i></a>
    </div>
  </footer>
  
</template>

<script>
export default {
  name: 'FooterComp'
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  footer{
    position: relative;
    padding: 50px 0;
    height: 450px;
    background-color: $sections-color;
    .lists-container{
      ul{
        li{
          a{
            color: black;
          }
        }
      }
      .story{
        color: $sections-color;
      }
      .right-col{
        margin-left: 70px;
      }
      
    }
    .social{
      margin-bottom: 90px;
      .fa-brands{
        font-size: 27px;
        color: #b1b1b1;
        margin-right: 30px;
      }
    }
    .credits{
      color: #b1b1b1;
    }
    .return-up{
      position: absolute;
      bottom: 20px;
      right: 20px;
      width: 50px;
      height: 50px;
      background-color: $primary-color;
      border-radius: 50%;
      text-align: center;
      line-height: 50px;
      a{
        color: white;
      }
    }
  }

</style>