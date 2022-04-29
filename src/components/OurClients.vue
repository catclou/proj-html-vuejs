<template>
    <div>
        <SlideshowClients/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import SlideshowClients from './partials/SlideshowClients.vue'

export default {
    name: 'OurClients',
    components: {
        // HelloWorld
        SlideshowClients
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    div {
        height: 10vh;
        width: 100%;
        border: 2px solid rgb(255, 245, 109);
    }
</style>