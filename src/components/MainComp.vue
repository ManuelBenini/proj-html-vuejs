<template>

  <main>
    <div class="hero pt-5 text-center">
      <div class="container mb-container">
        <h2>Learn At Your Own Pace!</h2>
        <p>Get Teamed up with people of the same will.</p>
        <button>Get started for free</button>
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
  </main>
  
</template>

<script>
export default {
  name: 'MainComp'
}
</script>

<style lang="scss" scoped>

  .hero{
    background-color: #1f2154;
    color: white;
    max-height: 570px;
    .jumbo-images{
      overflow: hidden;
      height: 515px;
    }
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
</style>