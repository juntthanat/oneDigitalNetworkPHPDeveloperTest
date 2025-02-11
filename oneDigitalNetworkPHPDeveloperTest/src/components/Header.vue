<script setup>
import Menu from "../components/HeaderComponents/Menu.vue"
import MyCart from "../components/HeaderComponents/MyCart.vue"
</script>

<template>
  <div id="header">
    <img src="../assets/BB-logo.png" id="logo" alt="BB Logo" />
    <Menu/>
    <MyCart/>
  </div>
</template>

<style>
#header {
  height: 116px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  box-shadow: 0px 4px 12px rgb(0, 0, 0, 0.2);
  box-shadow: 0px 8px 24px rgb(0, 0, 0, 0.2);
  box-shadow: 0px 18px 32px rgb(0, 0, 0, 0.2);
  background-color: #ffffff;

  padding-left: 84px;
  padding-right: 84px;
  padding-top: 28px;
  padding-bottom: 28px;
}
#logo {
  height: 40.97px;
  width: 211px;
}
</style>
