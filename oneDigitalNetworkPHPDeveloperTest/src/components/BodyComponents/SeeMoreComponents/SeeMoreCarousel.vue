<script setup>
import SeeMoreCarouselImage from '../SeeMoreComponents/SeeMoreCarouselComponents/SeeMoreCarouselImage.vue';
const props = defineProps(['data'])

</script>

<template>
  <div id="seeMoreContainer">
    <div id="seeMoreTitle">{{ props.data.title }}</div>
    <div id="seeMoreCarousel">
        <SeeMoreCarouselImage v-for="(seeMore, index) in props.data.data" :data="props.data.data[index]"/>
    </div>
  </div>
</template>

<style>
#seeMoreContainer {
  height: 376px;
  width: 1143px;
  display: flex;
  flex-direction: column;
  gap: 20px;
}
#seeMoreTitle {
  height: 30px;
  width: 1143px;
  font-size: 20px;
  font-weight: 600;
}
#seeMoreCarousel {
  height: 326px;
  width: 1143px;
  display: flex;
  gap: 21px;

}
</style>
