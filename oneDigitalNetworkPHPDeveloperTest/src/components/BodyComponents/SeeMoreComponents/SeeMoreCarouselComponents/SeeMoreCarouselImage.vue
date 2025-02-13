<script setup>
import { computed } from "vue";
const props = defineProps(["data"]);

const asdf = computed(() => {
  return (
    "src" + props.data.imageDirectory.replaceAll("/..", "").replaceAll("..", "")
  );
});
console.log(props.data.imageDirectory);
</script>

<template>
  <div id="seeMoreCarouselImageContainer">
    <div id="seeMoreCarouselImageInnerContainer">
      <img :src="props.data.imageDirectory" className="seeMoreImage" />
      <div className="seeMoreDetailContainer">
        <div className="seeMoreDescriptionContainer">
          <div className="seeMoreTitle">{{ props.data.seeMoreTitle }}</div>
          <div className="seeMoreDescription">
            {{ props.data.seeMoreDescription }}
          </div>
        </div>
        <div className="seeMorePrice">{{ props.data.seeMorePrice }}</div>
        <div className="seeMoreAddToCart">ใส่ตะกร้า</div>
      </div>
    </div>
  </div>
</template>

<style>
#seeMoreCarouselImageContainer {
  height: 326px;
  width: 270px;
  padding: 16px;
  border: 1px #bdbdbd solid;
  border-radius: 10px;
}
#seeMoreCarouselImageInnerContainer {
  display: flex;
  flex-direction: column;
  gap: 11px;
}
.seeMoreImage {
  height: 133px;
  width: 238px;
  background-color: #ffffff;
}
.seeMoreDetailContainer {
  height: 150px;
  width: 238px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.seeMoreDescriptionContainer {
  height: 52px;
  width: 238px;
}
.seeMoreTitle {
  height: 30px;
  width: 238px;
  font-size: 20px;
  font-weight: 700;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
.seeMoreDescription {
  font-size: 14px;
  font-weight: 300;
}
.seeMorePrice {
  color: #4285f4;
  font-size: 24px;
  font-weight: 600;
}
.seeMoreAddToCart {
  height: 42px;
  width: 238px;
  background-color: #4285f4;
  border-radius: 4px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #ffffff;
}
</style>
