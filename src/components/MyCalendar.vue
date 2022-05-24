<template>
<div class="calendar">
  <span>Ноябрь 2021</span>
  <div class="logo">
    <img src="../assets/Calendar.svg" alt="">
  </div>
</div>
</template>

<script>
export default {
  name: "MyCalendar.vue"
}
</script>

<style scoped>
.calendar{
  display: flex;
  width: 200px;
  font-size: 14px;
  height: 48px;
  background: #fff;
  border-radius: 4px;
  border: 1px solid #D0CBF0;
  filter: drop-shadow(0px 0px 3px rgba(0, 0, 0, 0.25));
  border-radius: 4px;
  align-items: center;
  justify-content: space-between;
}
.calendar span{
  margin-left: 10px;
  color: #6A6C7B;
}
.calendar img{
  margin-right: 10px;
}
</style>