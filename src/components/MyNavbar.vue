<template>
  <div class="nav">
    <div class="nav-content">
      <div class="logo">
        <img src="../assets/standart.svg" alt="">
      </div>
      <div class="menu">
        <img src="../assets/monochrome.svg" alt="">
        <span>Сервисы</span>
      </div>
      <div class="search">
        <img src="../assets/Vector.svg" alt="">
        <span>Поиск</span>
      </div>
      <div class="right-side">
        <img src="../assets/Frame.svg" alt="">
        <img src="../assets/default.svg" alt="">
        <img src="../assets/Ellipse.svg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyNavbar.vue"
}
</script>

<style scoped>
.nav{
  background: #fff;
}
.nav-content{
  width: 100%;
  display: flex;
  align-items: center;
}
.right-side{
  position: absolute;
  right: 20px;
  margin-right: 0;
  display: flex;
  justify-content: space-between;
}
.right-side img{
  margin-left: 28px;
}
.menu{
  display: flex;
  align-items: center;
  margin-left: 40px;
}
.menu img{
  margin-right: 12px;
}
.search{
  display: flex;
  align-items: center;
  margin-left: 40px;
}
.search img{
  margin-right: 12px;
}
</style>