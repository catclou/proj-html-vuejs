<template>
    <div>
        <OurPlansCard/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import OurPlansCard from './partials/OurPlansCard.vue'

export default {
    name: 'OurPlans',
    components: {
        // HelloWorld
        OurPlansCard
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    div {
        height: 10vh;
        width: 100%;
        border: 2px solid blue;
    }
</style>