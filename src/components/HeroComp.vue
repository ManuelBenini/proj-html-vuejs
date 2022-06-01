<template>

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
  
</template>

<script>
  import AccentBtnComp from './AccentBtnComp.vue';

  export default {
    name: 'heroComp',
    components: {AccentBtnComp }
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

</style>