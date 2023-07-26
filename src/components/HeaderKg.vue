<template>
  <main-container>
    <div class="row">
        <div class="col-md-12 col-sm-12 mb-5 mt-5">
      <nav class="navbar navbar-expand-lg navbar-light p-0 ">
        <div class="container-fluid ">
        <div class="collapse collapse-fontsize navbar-collapse d-flex justify-content-between" id="navbarSupportedContent">
        <div class="fol d-block">
        <form class="d-flex mb-3" role="search">
          <input class="form-control me-2" type="text" placeholder="HELLO, YOU CAN LOGIN OR REGISTER" aria-label="Search">
          <button class="btn btn-warning" type="submit">REGISTER</button>
        </form>
             <a class="navbar-brand logo" href="/"><img class="kgh" src="../assets/images/shopia/call__001_555_801___3895.png" alt="logo" /><i class="fa-solid fa-phone aq"></i></a>
          <form class="d-flex mt-3" role="search">
            <input class="form-control me-2" type="search" placeholder="SEARCH" aria-label="Search">
          </form>
        </div>
        <div class="cont">
            <a href="#"><img class="cd"  src="../assets/images/arrivel/ellipse_1_882.png" alt=""></a>
            <div class="centered mb-1">Your Logo</div>
            <div class="centered1">ECOMMERCE</div>
            </div>
            <div class="icons">
          <div class="fol d-block">
            <div class="d-flex mb-5">
               <a class="navbar-brand logo" href="/"><img class="kgh" src="../assets/images/shopia/call__001_555_801___3895.png" alt="logo" /></a>
               <a class="navbar-brand logo" href="/"><img class="kgh" src="../assets/images/arrivel/shopping_cart____34500_82.png" alt="logo" /></a>
               </div>
               <div class="d-flex justify-content-around mb-5">
                <div>
                  <a href="#"><img class="qwe" src="../assets/images/arrivel/flat_shoes__18900_690.png" alt=""></a>
                </div>
                <div>
                  <a href="#"><img class="erw" src="../assets/images/arrivel/hot_pants__15600_703.png" alt=""></a>
                </div>
               </div>
                      <form class="d-flex mb-3" role="search">
              <input class="form-control me-2" type="text1" placeholder="SHOW ALL PRODUCTS" aria-label="Search">
              <button class="btn btn-warning" type="submit">CHECK</button>
            </form>
          </div>
            </div>
          </div>
          </div>
      </nav>
    </div>
      <div class="col-md-12">
  <nav class="navbar navbar-expand-lg navbar-light p-0 ">
    <div class="container-fluid">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mx-auto mb-lg-0">
          <li class="nav-item menu-link" v-for="(menu, index) in headerMenuList" :key="index">
            <router-link
            class="nav-link me-5 active" aria-current="page"
            :to="menu.path">
              {{ menu.name }}
            </router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  </div>
  </div>
  </main-container>
</template>

<script>
import  {menuList, menuList2 } from '../constants/menuLinks'
import MainContainer from './MainContainer.vue'
export default {
  components: { MainContainer },
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: menuList,
      headerMenuLists: menuList2,
    }
  },
}
</script>

<style lang="scss">
@import '../assets/layouts/index';

.navbar {
  height: 90px;
}
.nav-link{
font-family: 'Source Sans Pro';
font-size: 15px;
line-height: 1.2;
font-weight: 600;
letter-spacing: 0.1em;
color: #444444;
}

.navbar-nav {
  height: 90px;
}

.logo {
  padding-right: 180px;
}

.collapse-fontsize {
  font-size: 18px;
}
.menu-link{
  font-family: Lato;
font-size: 11px;
line-height: 18px;
font-weight: 400;
color: #393939;
}

.menu-link1 {
font-family: Playfair;
font-size: 18px;
line-height: 17px;
font-weight: 400;
font-style: italic;
color: #000000;
  padding: 25px 30px;

  &:hover {
    background: grey;
  }
}

.icons {
  a {
    width: 20px;
    height: 20px;
    text-align: center;
    margin-right: 7px;
    display: inline-block;
  }
}

@media only screen and (max-width: 767px) {
  .icons {
 display: none;
  }
}
a .kgh{
font-weight: bold;
    position: relative;
    padding-right: 20px;

}
a .kgh:before{
    content: "\f041";
    font-family: FontAwesome;
    position: absolute;
    top: 0;
    left: 0;
}
.icons a{
  margin-right: 50px;
}
.ds{
  max-width: 30px;
}
.cd{
  max-width: 170px;

}
@media only screen and (max-width: 767px) {
  .cd {
   display: none;
  }
}
input[type=text] {
  background-color: rgb(255, 255, 255);
  background-image: url('../assets/images/arrivel/user_icon.png');
  background-position: 10px 10px;
  background-repeat: no-repeat;
  padding-left: 40px;
}
input[type=text1] {
  background-color: rgb(18, 15, 15);
  background-image: url('../assets/images/arrivel/plus.png');
  background-position: 10px 12px;
  background-repeat: no-repeat;
  padding-left: 40px;
   &::placeholder{
color: #fff;
  }
}
input[type=search] {
  background-color: rgb(255, 255, 255);
  background-image: url('../assets/images/arrivel/search_icon_731.png');
  background-position: 10px 10px;
  background-repeat: no-repeat;
  padding-left: 40px;


}
.qwe{
  background-color: rgb(255, 255, 255);
  background-image: url('../assets/images/arrivel/placehold_699.png');
  background-position: -20px 10px;
  background-repeat: no-repeat;
  padding-left: 40px;

}
.erw{
  background-color: rgb(255, 255, 255);
  background-image: url('../assets/images/arrivel/placehold_706.png');
  background-position: -20px 10px;
  background-repeat: no-repeat;
  padding-left: 40px;
}
.cont {
    position: relative;
    text-align: center;
    color: white;
}
.centered {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-weight: 500;


}
.centered1 {
    position: absolute;
    top: 60%;
    left: 50%;
    transform: translate(-50%, -50%);
    ont-family: 'Josefin Sans';
font-size: 8.2px;

font-weight: 700;
letter-spacing: 0.2em;
color: #ffffff;
}

</style>

