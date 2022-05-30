<template>

  <footer class="position-relative">

    <div class="container mb-container">

      <div class="lists-container d-flex">

        <ul v-for="(menu, index) in menuLists" :key="`menu${index}`" :class="menu.ulClass">
          <li :class="menu.liClass"><h5>{{menu.title}}</h5></li>
          <li v-for="(text, counter) in menu.text" :key="`text${counter}`">
            <p>{{text}}</p>
          </li>
        </ul>

      </div>

      <div class="social">

        <ul class="d-flex">
          <li v-for="(icon, index) in socialList" :key="`icon${index}`">
            <a href="#" v-html="icon"></a>
          </li>
        </ul>

      </div>

      <div class="credits text-center">
        <p>&copy; 2020 Maxcoach. All Rights Reserved</p>
      </div>

    </div>

    <div class="return-up">
     <a href="#"><i class="bi bi-arrow-up"></i></a>
    </div>

  </footer>
  
</template>

<script>
export default {
  name: 'FooterComp',
  props:{
    menuLists: Array,
    socialList: Array
  }
}
</script>

<style lang="scss" scoped>
  @import '../assets/style/variables';

  footer{
    padding: 50px 0;
    height: 450px;
    background-color: $sections-color;
    .lists-container{
      p{
        margin: 0;
        margin-top: 16px;
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
      font-size: 27px;
      a{
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
      font-size: 20px;
      &:hover{
      background-color: #3f3a64;
      }
      &:hover a{
      color: white;
      }
    }
  }
</style>