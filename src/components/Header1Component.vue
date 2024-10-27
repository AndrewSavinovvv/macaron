<script setup>

</script>

<template>
    <div class="header1 ">
      <div class="header1__main container">
        <div> <img src="@/assets/headerIMG/arrow-left.png" alt=""></div>
        <div class="header1__title">
          <img class="header1__title__img" src="@/assets/headerIMG/nuts.png" alt="">
          <span class="header1__title__mini">100%</span>
          <div class="header1__title__more">МИНДАЛЬНАЯ МУКА И НАТУРАЛЬНЫЕ ИНГРЕДИЕНТЫ</div>
        </div>
        <div><img src="@/assets/headerIMG/arrow-right.png" alt=""></div>
      </div>
    </div>
</template>

<style scoped>
.header1 {
  background: #D4E9F9;
  padding: 15px 12px;
}
.header1__title {
  position: relative;
  display: flex;
  align-items: center;
  font-size: 18px;
  color: black;
  font-weight: 400;
}
.header1__title__mini {
  position: absolute;
  bottom: 0;
  left: 15px;
  background: #6DCBBA;
  font-size: 11px;
  font-weight: 700;
  border-radius: 10px;
  padding: 2px 5px;
}
.header1__title__more {
  margin-left: 39px;
}
.header1__title__img {
  position: relative;
}
.header1__main {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
@media  (max-width: 834px) {
  .header1 {
    display: none;
  }
}
</style>