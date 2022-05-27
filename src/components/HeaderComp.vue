<template>

  <header>
    <div class="container mb-container h-100 d-flex justify-content-between align-items-center">
      <div class="logo flex-grow-1">
        <img src="../assets/img/light-logo.png" alt="logo Max Coach">
      </div>

      <div class="list">
        <ul class="d-flex align-items-center">
          <li class="d-flex">
            <a href="#">Home</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div> 
          </li>
          <li class="d-flex">
            <a href="#">Pages</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div> 
          </li>
          <li class="d-flex">
            <a href="#">Courses</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div> 
          </li>
          <li class="d-flex">
            <a href="#">Features</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div> 
          </li>
          <li class="d-flex">
            <a href="#">Blog</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div> 
          </li>
          <li class="d-flex position-relative">
            <a href="#">Shop</a>
            <div class="chevron"><i class="fa-solid fa-chevron-down"></i></div>
            <i class="fa-solid fa-cart-shopping"></i>
            <div class="shop-counter">0</div>
          </li>
          <li class="user">
            <a href="#"><i class="fa-regular fa-user"></i></a>
          </li>
        </ul>
      </div>

      <div class="search position-relative">
        <input type="text" placeholder="Search...">
        <i class="fa-solid fa-magnifying-glass"></i>
        
      </div>
    </div>
  </header>
  
</template>

<script>
export default {
  name: 'HeaderComp'
}
</script>

<style lang="scss" scoped>

  header{
    height: 60px;
    background-color: #1f2154;
    color: white;
    img{
      width: 150px;
      height: 100%;
    }
    li{
      margin-left: 55px;
      a{
        color: white;
      }
      .fa-user{
        font-size: 13px;
        text-align: center;
        padding-top: 1px;
        height: 18px;
        width: 18px;
        border: 2px solid white;
        border-radius: 50%;
      }
      .chevron{
        line-height:20px;
        padding-left: 6px;
        .fa-chevron-down{
          font-size: 8px;
        }
      }
      .fa-cart-shopping{
        line-height: inherit;
        padding-left: 10px;
      }
      .shop-counter{
        position: absolute;
        top: -5px;
        right: -10px;
        width: 13px;
        height: 13px;
        border: 1px solid white;
        background-color: white;
        color: black;
        text-align: center;
        line-height: 10px;
        font-size: 11px;
        border-radius: 50%;
      }
    }
    .user{
      margin-left: 25px;
      margin-right: 15px;
    }
    .search{
      input{
        border: none;
        border-radius: 5px;
        height: 40px;
        width: 180px;
        padding-left: 20px;
        padding-bottom: 5px;
      }
      i{
        position: absolute;
        top: 13px;
        right: 15px;
        font-size: 14px;
        color: green;
      }
    }
  }
</style>