<template>
<div class="my-select">
  <div class="label">{{label}}</div>
  <select name="" id="">
    <option :key="item" v-for="item in options" value="item">{{item}}</option>
  </select>
</div>
</template>

<script>
export default {
  name: "MySelect.vue",
  props:['options','label']
}
</script>

<style scoped>
.my-select{
  position: relative;
}
select{
  padding-top: 15px;
  width: 200px;
  font-size: 14px;
  height: 48px;
  border-radius: 4px;
  border: 1px solid #D0CBF0;
  filter: drop-shadow(0px 0px 3px rgba(0, 0, 0, 0.25));
  border-radius: 4px;
  padding-left: 5px;
  margin-right: 16px;

}
.label{
  top:7px;
  margin-left: 10px;
  position: absolute;
  font-size: 12px;
  color: #6153CC;
  z-index: 1000;
}
</style>