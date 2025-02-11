<script setup>
const props = defineProps(["type", "logoSrc", "typeList", "cssClass"]);
</script>
<template>
  <div id="dropDownContainer" :className="cssClass">
    <div id="titleContainer">
      <img :src="logoSrc" id="image" />
      <div id="textContainer">{{ props.type }}</div>
    </div>
    <div id="dropDownLogo">
        <img src="../../../../assets/ArrowDown.png"/>
    </div>
  </div>
</template>
<style>
#dropDownContainer {
  height: 42px;
  width: 312px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
#titleContainer {
  display: flex;
  padding-left: 16px;
  align-items: center;
  gap: 12px;
}
#image {
  height: 24px;
  width: 24px;
}
#textContainer {
  font-size: 14px;
}
#dropDownLogo{
    padding-right: 12px;
    height: 24px;
    width: 24px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.white{
    background-color: #FFFFFF;
    border: 1px #DEDEDE solid;
    border-radius: 8px;

}
.grey{
    background-color: #EBEBEB;
    border: 1px #DEDEDE solid;
    border-radius: 8px;
}
</style>
