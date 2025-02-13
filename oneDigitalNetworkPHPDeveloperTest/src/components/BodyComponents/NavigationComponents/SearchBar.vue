<script setup>
import DropDown from "./SearchBarComponents/DropDown.vue";
import brandImg from "../../../assets/Brand.png";
import filterImg from "../../../assets/Filter.png";

const typeList = ['type1', 'type2', 'type3']
</script>
<template>
  <div id="searchBar">
    <div id="productName">Work Louder: Nomad [E] Mechanical Keyboard</div>
    <div id="searchBarText">ค้นหาผลิตภัณฑ์</div>
    <div id="filterDropDown">
      <DropDown
        type="เลือกแบรนด์"
        :logoSrc="brandImg"
        :typeList
      />
      <DropDown
        type="เลือกผลิตภัณฑ์"
        :logoSrc="filterImg"
        :typeList
      />
    </div>
    <div id="searchButtonContainer">
      <button id="searchButton">ค้นหา</button>
      <div id="resetContainer">
        <button id="resetButton">รีเซ็ต</button>
        <img
          src="../../../assets/RefreshOutline.png"
          id="refresh"
          alt="refresh outline"
        />
      </div>
    </div>
  </div>
</template>
<style>
#searchBar {
  height: 259px;
  width: 1129px;
  position: absolute;
  top: 245px;
  background-color: #f4f8ff;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 21px;
  z-index: 1;
  border-radius: 10px;
}
#productName {
  font-size: 24px;
  font-weight: 700;
}
#searchBarText {
  height: 44px;
  width: 645px;
  font-size: 20px;
  font-weight: 600;
  display: flex;
  align-items: center;
  justify-content: center;
}
#filterDropDown {
  height: 42px;
  width: 645px;
  display: flex;
  gap: 21px;
}
#searchButtonContainer {
  position: relative;
  height: 44px;
  width: 645px;
  padding-left: 154px;
  display: flex;
  gap: 21px;
  z-index: 1;
}
#searchButton {
  position: relative;
  height: 44px;
  width: 341px;
  border-radius: 8px;
  background-color: #4285f4;
  color: #ffffff;
  font-weight: 700;
  z-index: 1;
}
#resetContainer {
  position: relative;
  height: 44px;
  width: 54px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  z-index: 1;
}
#resetButton {
  font-size: 12px;
  color: #505050;
}
#refresh {
  height: 24px;
  width: 24px;
}
</style>
