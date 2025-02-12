<script setup>
    import Navigation from '../components/BodyComponents/Navigation.vue'
    import Carousel from './BodyComponents/Carousel.vue';
</script>

<template>
    <div id="bodyContainer">
        <div id="navigate">
            <Navigation/>
        </div>
        <div id="carousel">
            <Carousel/>
        </div>
    </div>
</template>

<style>
#bodyContainer{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 33px;
}
#navigate{
    display: flex;
    justify-content: center;
    align-items: center;
}
#carousel{

}
</style>