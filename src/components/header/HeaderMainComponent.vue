<script setup>

</script>

<template>
  <div class="header2">
    <div class="header2__main container">
      <div class="header2__main__nav">
        <ul class="header2__main__nav__list">
          <li>Гарантия свежести</li>
          <li>Доставка и оплата</li>
          <li>Оптовые поставки</li>
          <li>Контакты</li>
        </ul>
      </div>
      <div class="header2__main__contact">
        <ul class="header2__main__contact__list">
          <li>
            <img src="../../assets/headerIMG/geo.png" alt="">
            <span>Санкт-Петербург</span>
            <img src="../../assets/headerIMG/arrow-down.png" alt="">
          </li>
          <li>
            <img src="../../assets/headerIMG/phone.png" alt="">
            <span>8 812 309-82-88</span>
          </li>
          <li>
            <img src="../../assets/headerIMG/bag2.png" alt="">
            <span>В корзине (4 товара)</span>
          </li>
        </ul>
      </div>
      <div class="header2__main__social">
        <ul class="header2__main__social__list">
          <li>
            <img src="../../assets/headerIMG/tg.png" alt="">
          </li>
          <li>
            <img src="../../assets/headerIMG/vk.png" alt="">
          </li>
          <li>
            <img src="../../assets/headerIMG/ok.png" alt="">
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
.header2 {
  display: flex;
  background: #F7EBE5;
  padding: 0;
  margin: 0;
}

.header2__main {
  display: flex;
  font-size: 14px;
  font-weight: 400;
  white-space: nowrap;
  align-items: center;
  justify-content: space-between;
}

.header2__main__nav__list,
.header2__main__contact__list,
.header2__main__social__list {
  display: flex;
  list-style: none;
  gap: 10px;
  padding: 0;

}

.header2__main__nav__list li,
.header2__main__contact__list li,
.header2__main__social__list li {
  display: inline-flex;
  align-items: center;
  gap: 10px;
}
@media  (max-width: 1026px) {
  .header2 {
    display: none;
  }
}
</style>