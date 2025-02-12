<script setup>
import { ref } from "vue";
const props = defineProps(["image"]);

let index = ref(0);

function increment() {
  index.value++;
  index.value = index.value % 6;
}

function decrement() {
  if (index.value == 0) {
    index.value = 5;
  } else {
    index.value--;
  }
}
</script>

<template>
  <div id="galleryHeroContainer">
    <img :src="props.image[index]" id="galleryImage" />
    <div id="galleryNav">
      <button className="galleryNavArrow" @click="decrement">
        <img src="../../../assets/CarouselImage/RightArrow.svg" />
      </button>
      <button className="galleryNavArrow" @click="increment">
        <img
          src="../../../assets/CarouselImage/RightArrow.svg"
          className="rotate"
        />
      </button>
    </div>

    <img src="../../../assets/Sale.png" id="saleImage" />
  </div>
</template>

<style>
#galleryHeroContainer {
  height: 281px;
  width: 450px;

  background-color: #dedede;
}
#galleryImage {
  height: 281px;
  width: 450px;
}
#galleryNav {
  height: 34px;
  width: 482px;
  position: relative;
  top: -50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  justify-content: space-between;
}
.galleryNavArrow {
  height: 34px;
  width: 34px;
  border-radius: 100%;

  /* box-shadow: 1px 2px 8px #b3b3b3; */

  box-shadow: 0px 3.48px 6.95px rgba(0, 0, 0, 0.1),
    0px 13.9px 27.81px rgba(0, 0, 0, 0.1),
    0px 20.86px 55.62px rgba(0, 0, 0, 0.1);
}
.rotate {
  rotate: 180deg;
}
#saleImage {
  height: 44px;
  width: 101px;
  position: absolute;
  top: 12px;
  left: 12px;
}
</style>
