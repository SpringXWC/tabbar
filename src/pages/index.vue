<template>
  <div>
    <tabbar v-model="select">
      <tabbar-item id="homePage">
        <img src="../assets/image/homePage.png" slot="icon-normal">
        <img src="../assets/image/homePage_select.png" slot="icon-active">
        首页
      </tabbar-item>
      <tabbar-item id="service">
        <img src="../assets/image/service.png" slot="icon-normal">
        <img src="../assets/image/service_select.png" slot="icon-active">
        客服中心
      </tabbar-item>
      <tabbar-item id="message">
        <img src="../assets/image/message.png" slot="icon-normal">
        <img src="../assets/image/message_select.png" slot="icon-active">
        消息中心
      </tabbar-item>
      <tabbar-item id="personal">
        <img src="../assets/image/personal.png" slot="icon-normal">
        <img src="../assets/image/personal_select.png" slot="icon-active">
        个人中心
      </tabbar-item>
    </tabbar>
  </div>
</template>
<script>
  import tabbar from '../components/tabbar';
  import tabbarItem from '../components/tabbarItem';
  export default{
    components:{
      tabbar,
      tabbarItem
    },
    data(){
      return{
        select:'homePage'
      }
    }
  }
</script>
