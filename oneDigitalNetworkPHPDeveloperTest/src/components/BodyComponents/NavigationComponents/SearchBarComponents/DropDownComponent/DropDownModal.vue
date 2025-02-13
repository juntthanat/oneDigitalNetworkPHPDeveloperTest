<script setup>
const props = defineProps(["typeList", "handleClick"]);
</script>

<template>
  <div id="fullPageModal" @click="handleClick"></div>
  <div id="modalContainer">
    <div v-for="type in props.typeList" class="dropDownSelector" @click="handleClick">
        {{ type }}
    </div>
  </div>
</template>

<style>
#modalContainer {
  position: relative;
  max-height: 168px;
  width: 312px;
  overflow: auto;
  z-index: 2;

  background-color: #ffffff;
}
#fullPageModal {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 1;

  background-color: rgba(0, 0, 0, 0.3);
}
.dropDownSelector:hover {
    background-color: lightgrey;
}
</style>
