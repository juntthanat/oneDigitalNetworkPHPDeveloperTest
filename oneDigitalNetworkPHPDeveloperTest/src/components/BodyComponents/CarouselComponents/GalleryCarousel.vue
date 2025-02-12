<script setup>
const props = defineProps(['imageCarousel'])
</script>

<template>

<div id="galleryCarousel">
    <img :src="props.imageCarousel[0]" className="carouselImage"/>
    <img :src="props.imageCarousel[1]" className="carouselImage"/>
    <img :src="props.imageCarousel[2]" className="carouselImage"/>
    <img :src="props.imageCarousel[3]" className="carouselImage"/>
    <img :src="props.imageCarousel[4]" className="carouselImage"/>
    <img :src="props.imageCarousel[5]" className="carouselImage"/>
</div>
</template>

<style>
#galleryCarousel{
    height: 46.39px;
    width: 448.48px;
    display: flex;
    justify-content: space-between;


    /* background-color: aquamarine; */
}
.carouselImage{
    height: 46px;
    width: 68px;
}
</style>