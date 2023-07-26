<template>
  <div class="arrivals">
    <div class="container">
     <div class="el el-1">
      <a href="#"><img class="fot1" src="../assets/images/arrivel/deva2.png" alt=""></a>
     </div>
     <div class="el el-2">
      <a href="#"><img class="fot2" src="../assets/images/arrivel/deva12.jpg" alt=""></a>
     </div>
     <div class="el el-3">
      <a href="#"><img class="fot3" src="../assets/images/arrivel/deva11.jpg" alt=""></a>
     </div>
     <div class="el el-4">
      <a href="#"><img class="fot4" src="../assets/images/arrivel/deva5.png" alt=""></a>
     </div>
     <div class="el el-5">
      <a href="#"><img class="fot5" src="../assets/images/arrivel/deva4.png" alt=""></a>
     </div>
  </div>
  </div>
</template>
<style lang="scss">
.el {
   padding: 15px 35px;
   font-size: 21px;
   color: #fff;

}
.container {
   display: grid;
   grid-template:
   'aside header header home' 280px
   'aside main footer footer' 280px;
   gap: 7px;
}

@media only screen and (max-width: 767px) {
  .container {
    grid-template-areas:
        "aside"
        "aside"
        "aside"
        "header"
        "home"
        "main"
        "footer";
  }
}
.el-1 {
   grid-area: header;
}
.el-2 {
   grid-area: aside;
}
.el-3 {
   grid-area: main;
}
.el-4 {
   grid-area: footer;
}
.el-5 {
   grid-area: home;
}

.fot1{
  object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform: scale(1.2);
        }
}
.fot2{
 object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform: scale(1.2);
        }
}
.fot3{
 object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform: scale(1.2);
        }
}
.fot4{
  object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform: scale(1.2);
        }
}
.fot5{

  object-fit: cover;
        width: 100%;
        height: 100%;
        transition: 1s;
        &:hover{
          transform: scale(1.2);
        }
}

 .arrivals{
   margin-bottom: 60px;
 }
</style>