<template>
  <MyNavbar/>
  <MyContainer>
    <SideNav :dashboard="Dashboard"/>
    <div class="main-content">
      <div class="first-row">
        <span>Капитализация</span>
        <div class="buttons">
          <MySelect :label="label[0]" :options="options"/>
          <MySelect :label="label[1]" :options="options2"/>
          <MyCalendar/>
          <MyDownload/>
        </div>
      </div>

      <div class="second-row">
        <MyTable :label="'ORGCITY PLANNING  (EI.0.0B2B.2021.30)'" :row="row" :head="head"/>
      </div>

    </div>

  </MyContainer>

</template>

<script>


import MyNavbar from "@/components/MyNavbar";
import SideNav from '@/components/SideNav'
import MyContainer from '@/components/MyContainer'
import MySelect from '@/components/MySelect'
import MyCalendar from '@/components/MyCalendar'
import MyDownload from '@/components/MyDownload'
import MyTable from '@/components/MyTable'

export default {
components: {MyTable, MyDownload, MyCalendar, MySelect, MyContainer, SideNav, MyNavbar},
  data(){
  return{
    Dashboard: [
      {
        title: ['', '', '', ''],
      }
    ],
    options:['Менеджер','Директор','Стажер'],
    label:['Роль','Продукты'],
    options2: ['Все','продукт1', 'Продукт2'],
    head:['ФИО','Роль', 'Тип бюджета', 'Занятость', 'Факт', 'Корректировка'],
    row: ['Федоров Сергей Михайлович', 'Менеджер проектов', 'OPEX', '100%', '60%', '50%']
  }
  }
}
</script>

<style>
body{
  margin: 0;
  background: #F8F8F9;
  font-family: 'Roboto';
  font-style: normal;
  padding: 0;
  overflow: hidden;
}
.main-content{
  width: 100%;
}
.first-row{
  font-size: 24px;
  margin-left: 40px;
  margin-top: 40px;
  display: flex;
  justify-content: space-between;
  max-height: 90px;
}
.second-row{
  margin-left: 40px;
}
.buttons{
  display: flex;
  width: 700px;
}
</style>
