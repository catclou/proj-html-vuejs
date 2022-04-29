<template>
    <div>
        <MeetCard/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import MeetCard from './partials/MeetCard.vue'

export default {
    name: 'MeetSection',
    components: {
        // HelloWorld
        MeetCard
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