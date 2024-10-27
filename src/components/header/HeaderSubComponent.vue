<script setup>

</script>

<template>
  <div class="header3">
    <div class="header3__main container">
     <div class="header3__main__block">
       <ul class="header3__list">
       <li class="header3__list__item">
         <span>СЛАДКИЕ ДНИ</span>
         <img src="../../assets/headerIMG/sale.png" alt="">
       </li>
       <li class="header3__list__item">
         <span>ПОДАРОЧНЫЕ НАБОРЫ</span>
         <img src="../../assets/headerIMG/arrow-down.png" alt="">
       </li>
       <li class="header3__list__item">СОБРАТЬ НАБОР</li>
       <li class="header3__list__item">
         <img src="../../assets/headerIMG/лого.png" alt="">
       </li>
       <li class="header3__list__item">СОЗДАТЬ ДИЗАЙН</li>
       <li class="header3__list__item">
         <span>КОМПАНИЯМ</span>
         <img src="../../assets/headerIMG/arrow-down.png" alt="">
       </li>
       <li class="header3__list__item">
         <span>ВЕСЬ КАТАЛОГ</span>
         <img src="../../assets/headerIMG/arrow-down.png" alt="">
       </li>
     </ul></div>
    </div>
  </div>
</template>

<style scoped>
.header3 {
  max-width: 1600px;
  padding-left: 50px;
}
.header3__list {
  display: flex;
  list-style: none;
  align-items: center;
  justify-content: space-between;
  padding: 0;
  margin: 0;
}
.header3__list__item {
  display: flex;
  align-items: center;
  white-space: nowrap;
  font-size: 14px;
  font-weight: 400;
  padding-top: 19px;
}
.header3__list__item span {
  color: #2B1414;
  padding-right: 5px;
}
.header3__main {
 padding-left: 250px;
}
@media  (max-width: 1026px) {
  .header3 {
    display: none;
  }
}
@media  (max-width: 1440px) {
  .header3__main {
    padding-left: 50px;
    max-width: 0;
  }
}
</style>