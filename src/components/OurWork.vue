<template>
    <div>
        <OurWorkImg/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import OurWorkImg from './partials/OurWorkImg.vue'

export default {
    name: 'OurWork',
    components: {
        // HelloWorld
        OurWorkImg
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    div {
        height: 10vh;
        width: 100%;
        border: 2px solid green;
    }
</style>