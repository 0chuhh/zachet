<template>
<div class="side-nav">
  <div class="logo">
    <img src="../assets/sidenav.svg" alt="">
  </div>
  <div class="menu">
    <div class="menu-item">
      <div class="item-logo">
        <img src="../assets/home.svg" alt="">
      </div>
    </div>

    <div class="menu-item">
      <div class="item-logo">
        <img src="../assets/Icon_Sataffing.svg" alt="">
      </div>
    </div>

    <div class="menu-item">
      <div class="item-logo">
        <img src="../assets/Iconside2.svg" alt="">
      </div>
    </div>

    <div class="menu-item">
      <div class="item-logo">
        <img src="../assets/Iconside3.svg" alt="">
      </div>
    </div>
  </div>
</div>
</template>

<script>

export default {


}
</script>

<style scoped>
.nav{
  overflow: hidden;
}
.side-nav{
  width: 56px;
  height: 100vh;
  background: #D0CBF0;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  flex-direction: column;
}
.logo{
  margin-top: 20px;
}
.menu{
  width: 100%;
  margin-top: 38px;
  height: 25vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}
.menu-item{
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 50px;
}
.item-logo{
  display: flex;
  justify-content: center;
}
.menu-item:hover{
  background: #938cb8;
}
</style>