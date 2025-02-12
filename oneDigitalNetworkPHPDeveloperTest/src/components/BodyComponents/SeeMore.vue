<script setup>
import SeeMoreCarousel from './SeeMoreComponents/SeeMoreCarousel.vue'
import json from '../../assets/SeeMoreData/SeeMoreData.json'


// console.log(json.data.sameCompany.data[0].imageDirectory)
</script>

<template>
    <div id="seeMoreContainer" >
        <SeeMoreCarousel :data="json.data.sameCompany"/>
        <SeeMoreCarousel :data="json.data.similarProduct"/>
    </div>

</template>

<style>
    #seeMoreContainer{
        height: 100%;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 32px;
    }
</style>