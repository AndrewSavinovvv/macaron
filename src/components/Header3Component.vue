<script setup>

</script>

<template>
  <div class="header3">
    <div class="header3__main container">
      <ul class="header3__list">
        <li class="header3__list__item">
          <span>СЛАДКИЕ ДНИ</span>
          <img src="@/assets/headerIMG/sale.png" alt="">
        </li>
        <li class="header3__list__item">
          <span>ПОДАРОЧНЫЕ НАБОРЫ</span>
          <img src="@/assets/headerIMG/arrow-down.png" alt="">
        </li>
        <li class="header3__list__item">СОБРАТЬ НАБОР</li>
        <li class="header3__list__item">
          <img src="@/assets/headerIMG/лого.png" alt="">
        </li>
        <li class="header3__list__item">СОЗДАТЬ ДИЗАЙН</li>
        <li class="header3__list__item">
          <span>КОМПАНИЯМ</span>
          <img src="@/assets/headerIMG/arrow-down.png" alt="">
        </li>
        <li class="header3__list__item">
          <span>ВЕСЬ КАТАЛОГ</span>
          <img src="@/assets/headerIMG/arrow-down.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.header3 {
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
  margin-top: 19px;
  margin-left: 30px;
  white-space: nowrap;
}
.header3__list__item span {
  font-size: 14px;
  font-weight: 400;
}
@media  (max-width: 834px) {
  .header3 {
    display: none;
  }
}
</style>