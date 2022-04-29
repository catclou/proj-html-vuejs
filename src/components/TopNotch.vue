<template>
    <div>
        <TopNotchCard/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import TopNotchCard from './partials/TopNotchCard.vue'

export default {
    name: 'TopNotch',
    components: {
        // HelloWorld
        TopNotchCard
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    div {
        height: 10vh;
        width: 100%;
        border: 2px solid orange;
    }
</style>