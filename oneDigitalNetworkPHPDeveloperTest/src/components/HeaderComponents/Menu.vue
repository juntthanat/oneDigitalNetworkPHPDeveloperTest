<script setup>
import { ref } from "vue";
const currentSelectedMenu = ref(0);
const selectedMenu = "menuSelection selected";
const unSelectedMenu = "menuSelection";

function checkSelected(id) {
  let selected = false;
  if (currentSelectedMenu.value == id) {
    selected = true;
  } else {
    selected = false;
  }
  return selected ? selectedMenu : unSelectedMenu;
}
</script>

<template>
  <div id="menu">
    <button :className="checkSelected(1)" @click="currentSelectedMenu = 1">
      หน้าหลัก
    </button>
    <button :className="checkSelected(2)" @click="currentSelectedMenu = 2">
      สินค้าใหม่
    </button>
    <button :className="checkSelected(3)" @click="currentSelectedMenu = 3">
      อุปกรณ์ไอที
    </button>
  </div>
</template>

<style>
#menu {
  height: 60px;
  width: 383px;
  background-color: #e8f0fe;
  border-radius: 55px;
  padding: 4px;

  display: flex;
  align-items: center;
  justify-content: space-evenly;
  gap: 30px;
}
.menuSelection {
  height: 52px;
  width: 117px;
  color: #5a5a5a;
  border-radius: 34px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.selected {
  background-color: #4285f4;
  color: #ffffff;
}
</style>
