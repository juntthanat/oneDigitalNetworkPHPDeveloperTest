<script setup>
import { ref } from "vue";
import DropDownModal from "./DropDownComponent/DropDownModal.vue";
const props = defineProps(["type", "logoSrc", "typeList"]);

const isActive = ref(true);

function handleClick() {
  isActive.value = !isActive.value;
}
</script>
<template>
  <div>
    <div
      id="dropDownContainer"
      class="white"
      @click="handleClick"
      :class="{ putToFront: !isActive }"
    >
      <div id="titleContainer">
        <img :src="logoSrc" id="image" />
        <div id="textContainer">{{ props.type }}</div>
      </div>
      <div id="dropDownLogo">
        <img src="../../../../assets/ArrowDown.png" />
      </div>
    </div>
    <div class="modalCSS" :class="{ showModal: isActive }">
      {{ console.log(isActive) }}
      <DropDownModal :typeList="props.typeList" :handleClick />
    </div>
  </div>
</template>
<style>
#dropDownContainer {
  position: relative;
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
#dropDownLogo {
  padding-right: 12px;
  height: 24px;
  width: 24px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.white {
  background-color: #ffffff;
  border: 1px #dedede solid;
  border-radius: 8px;
}

.showModal {
  display: none;
}
.modalCSS {
  position: relative;
  z-index: 4;
}
.putToFront {
  position: relative;
  z-index: 5;
}
</style>
