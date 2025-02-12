<script setup>
import Navigation from "../components/BodyComponents/Navigation.vue";
import Carousel from "./BodyComponents/Carousel.vue";
import SeeMore from "./BodyComponents/SeeMore.vue";
</script>

<template>
  <div id="bodyContainer">
    <div id="navigate">
      <Navigation />
    </div>
    <div id="carousel">
      <Carousel />
    </div>
    <div id="seeMore">
      <SeeMore />
    </div>
  </div>
</template>

<style>
#bodyContainer {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 33px;
}
#navigate {
  display: flex;
  justify-content: center;
  align-items: center;
}
#carousel {
}
#seeMore {
  height: 784px;
  width: 1143px;
  position: absolute;
  top: 1111px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
