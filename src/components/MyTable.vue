<template>
  <div class="label">

    {{label}}
    <img src="../assets/more.svg" alt="">
  </div>
  <table>
    <tr>
      <th :key="item" v-for="item in head">{{ item }}</th>
    </tr>
    <tr :key="item" v-for="item in [1,2,3,4,5,6,7]">
      <td :key="item1" v-for="item1 in row">{{item1}}</td>
    </tr>

  </table>
</template>

<script>
export default {
  name: "MyTable.vue",
  props:['head', 'row', 'label']
}
</script>

<style scoped>
table{
  margin-top: 16px;
  border-spacing: 0px;
  position: relative;
  padding-top: 50px;
  width: 876px;
  background: #FFFFFF;
  /* Xenia_shadow */

  box-shadow: 0px 0px 3px rgba(0, 0, 0, 0.25);
  border-radius: 12px;
}
td{
  max-width: 106px;
  height: 48px;
  padding: 12px;
}
th{
  padding: 12px;
  height: 48px;
  text-align: left;
  border: none;
  margin: 0;
  background: #E5E6E8;
}
.label{
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: absolute;
  z-index: 100;
  margin-top: 12px;
  margin-left: 12px;
  color: #2A2D43;
  font-weight: bold;
  font-size: 14px;
  line-height: 20px;
}
tr:nth-child(even){
  background: #ECEAF9;
}
</style>