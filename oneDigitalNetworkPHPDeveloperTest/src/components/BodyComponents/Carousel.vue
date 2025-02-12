<script setup>
import GalleryHero from "../BodyComponents/CarouselComponents/GalleryHero.vue";
import GalleryCarousel from "../BodyComponents/CarouselComponents/GalleryCarousel.vue";
import Description from '../BodyComponents/CarouselComponents/Description.vue'

import MainImage from '../../assets/CarouselImage/MainImage.png'
import Image1 from '../../assets/CarouselImage/Image1.png'
import Image2 from '../../assets/CarouselImage/Image2.png'
import Image3 from '../../assets/CarouselImage/Image3.png'
import Image4 from '../../assets/CarouselImage/Image4.png'
import Image5 from '../../assets/CarouselImage/Image5.png'
import Image6 from '../../assets/CarouselImage/Image6.png'

const mainImage = MainImage;
const carouselImage = [Image1, Image2, Image3, Image4, Image5, Image6]
</script>

<template>
  <div id="carouselContainer">
    <div id="carouselHeaderContainer">
      <div id="price">11,799 บาท</div>
      <div id="dataAndView">
        <img src="../../assets/Calender.png" alt="caledner" id="calender" />
        <div id="date">ข้อมูล ณ วันที่ 1 พ.ย. 67</div>
        <img src="../../assets/View.png" alt="view" id="view" />
        <div>45,959</div>
      </div>
    </div>
    <div id="sectionDivider"></div>
    <div id="gallery">
      <div id="galleryContainer">
        <GalleryHero :image="carouselImage"/>
        <GalleryCarousel :imageCarousel="carouselImage" />
      </div>
      <div id="description">
        <Description/>
      </div>
    </div>
  </div>
</template>

<style>
#price {
  height: 36px;
  width: 123px;

  font-size: 24px;
  font-weight: 700;

  color: #4285f4;
}
#carouselHeaderContainer {
  height: 36px;
  width: 1129px;
  position: absolute;
  top: 537px;
  display: flex;
  gap: 103px;
}
#carouselContainer {
  display: flex;
  justify-content: center;
  align-items: center;
}
#dataAndView {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
  color: #777777;
  font-size: 12px;
  font-weight: 500;
}
#calender {
  height: 24px;
  width: 24px;
}
#view {
  height: 24px;
  width: 24px;
  margin-left: 12px;
}
#sectionDivider {
  height: 0px;
  width: 1136px;
  border: 1px #e4e4e4 solid;

  position: absolute;
  top: 593px;
}
#gallery{
  width: 1136px;
  position: absolute;
  top: 639px;
  display: flex;
  gap: 62px;
}
#galleryContainer {
  display: flex;
  flex-direction: column;
  gap: 42px;
}
</style>
