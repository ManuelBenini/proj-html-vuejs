<template>

  <header>

    <div class="container mb-container h-100 d-flex justify-content-between align-items-center">

      <div class="logo flex-grow-1">
        <img src="../assets/img/light-logo.png" alt="logo Max Coach">
      </div>

      <div class="list">

        <ul class="d-flex align-items-center">
          <li v-for="(menu, index) in headerMenu" :key="`menu${index}`" :class="menu.liClass">
            <a v-if="menu.text" href="#">{{menu.text}}</a>
            <a v-else href="#" v-html="menu.userIcon"></a>

            <div v-if="menu.divClass" :class="menu.divClass" v-html="menu.chevron"></div>
            <div v-if="menu.shopIcon" class="shop" v-html="menu.shopIcon"></div>
            <div v-if="menu.shopCounter" class="shop-counter">{{menu.shopCounter}}</div>
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
    name: 'HeaderComp',
    props:{
      headerMenu: Array
    }
  }
</script>

<style lang="scss" scoped>

  header{
    height: 60px;
    background-color: #1f2154;
    color: white;
    img{
      width: 130px;
      height: 100%;
    }
    li{
      margin-left: 35px;
      font-weight: 400;
      font-size: 14px;
      .chevron{
        line-height:20px;
        padding-left: 6px;
        font-size: 8px;
      }
      .shop{
        margin-left: 5px;
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
        font-size: 10px;
        border-radius: 50%;
        font-weight: 400;
      }
    }
    .user{
      margin-left: 25px;
      margin-right: 18px;
      font-size: 11px;
      text-align: center;
      line-height: 14px;
      height: 15px;
      width: 15px;
      border: 2px solid white;
      border-radius: 50%;
    }
    
    .search{
      input{
        border: none;
        border-radius: 5px;
        height: 40px;
        width: 180px;
        padding-left: 20px;
        padding-bottom: 5px;
        &::placeholder{
          font-size: 14px;
        }
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