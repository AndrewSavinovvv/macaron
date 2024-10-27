<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value
}
</script>

<template>
  <div class="header-mobile">
    <div class="burger" @click="toggleMenu">
      <span class="short"></span>
      <span></span>
      <span></span>
    </div>

    <div class="logo">
      <img class="logo" src="../../assets/headerIMG/лого.png" alt="">
    </div>

    <div class="cart">
      <img src="../../assets/headerIMG/bag2.png" alt="">
    </div>
  </div>

  <div v-if="isMenuOpen" class="menu-overlay">
    <div class="menu">
      <button class="close-button" @click="toggleMenu">×</button>
      <ul>
        <li class="item__city">
          <img src="@/assets/headerIMG/geo.png" alt="">
          <span class="city">Санкт-Петербург</span>
          <img src="../../assets/headerIMG/arrow-down.png" alt="">
        </li>
        <li class="item__sale">
          <span class="sale">СЛАДКИЕ ДНИ</span>
          <img src="@/assets/headerIMG/sale.png" alt="">
        </li>
        <li class="item__gift">
          <span class="gift" >ПОДАРОЧНЫЕ НАБОРЫ</span>
          <img src="../../assets/headerIMG/arrow-down.png" alt="">
        </li>
        <li>СОБРАТЬ НАБОР</li>
        <li>СОЗДАТЬ ДИЗАЙН </li>
        <li class="item__company">
          <span class="company">КОМПАНИЯМ</span>
          <img src="../../assets/headerIMG/arrow-down.png" alt="">
        </li>
        <li  class="item__company">
          <span class="company">ВЕСЬ КАТАЛОГ</span>
          <img src="../../assets/headerIMG/arrow-down.png" alt="">
          </li>
        <li class="item__info">
          Гарантия свежести
        </li>
        <li class="item__info">Доставка и оплата</li>
        <li class="item__info">Оптовые поставки</li>
        <li class="item__info">Контакты</li>
        <li class="item__number">
          <img src="@/assets/headerIMG/phone.png" alt="">
          <span class="number">8 812 309-82-88</span>
        </li>
        <li class="item__social">
          <img class="vk" src="../../assets/headerIMG/tg.png" alt="">
          <img class="tg" src="../../assets/headerIMG/vk.png" alt="">
          <img class="ok" src="../../assets/headerIMG/ok.png" alt="">
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.header-mobile {
  display: none;
  align-items: center;
  justify-content: space-between;
  padding: 0 16px;
  height: 60px;
  background-color: #F7EBE5;
}

.burger {
  display: flex;
  flex-direction: column-reverse;
  justify-content: space-around;
  width: 24px;
  height: 18px;
  cursor: pointer;
}
.burger span {
  display: block;
  height: 2px;
  background-color: #000000;
  border-radius: 2px;
}
.burger span.short {
  width: 16px;
}

.logo {
  height: 56px;
  width: 56px;
}

@media (max-width: 1026px) {
  .header-mobile {
    display: flex;
  }
}

.menu-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: center;
}

.menu {
  background-color: #F7EBE5;
  width: 100%;
  height: 100%;
  padding: 16px;
  position: relative;
  overflow-y: auto;
}

.close-button {
  position: absolute;
  top: 20px;
  left: 18px;
  font-size: 56px;
  background: none;
  border: none;
  cursor: pointer;
}

.menu ul {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  align-items: center;
  list-style: none;
  padding: 0;
  margin: 60px 0 0;
}

.menu ul li {
  display: flex;
  justify-content: center;
  margin: 10px 0;
  font-size: 14px;
  color: #2B1414;
  font-weight: 400;
  width: 100%;
  border-bottom: 1px solid #0000001A;
  padding-bottom: 11px;

}
.city {
  font-weight: 600;
  font-size: 14px;
  color: #000000E0;
  padding-left: 5px;
  padding-right: 5px;
}
.item__city,.item__gift {
  display: flex;
  align-items: center;
}
.item__number {
  display: flex;
  align-items: center;
}
.number {
  padding-left: 5px;
  font-weight: 600;
  font-size: 14px;
}
.ok,.vk,.tg {
  padding-left: 10px;
}
.item__sale {
  display: flex;
  align-items: center;
}
.sale , .gift{
  padding-right: 5px;
}
.menu ul li.item__info {
  margin: 11px 0 !important;
  border: none;
}
.item__company {
  display: flex;
  align-items: center;
}
.company {
  padding-right: 5px;
}

.item__number{
  padding-top: 10px;
  border-top: 1px solid #0000001A;;
}
.item__social ,.item__number{
  border-bottom: none !important;
}
.item__social {
  margin: 0 !important;
}
</style>