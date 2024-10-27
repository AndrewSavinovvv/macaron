<script setup>

</script>

<template>
  <div class="header-mobile">

    <div class="burger">
      <span class="short"></span>
      <span></span>
      <span></span>
    </div>

    <div class="logo">
      <img class="logo" src="@/assets/headerIMG/лого.png" alt="">
    </div>
    
    <div class="cart">
      <img src="@/assets/headerIMG/bag2.png" alt="">
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
  height: 2px;
}

.logo {
  height: 56px;
  width: 56px;
}

.cart {

}
@media  (max-width: 834px) {
  .header-mobile {
    display: flex;
  }
}
</style>