<template>
    <div>
        <NewsPost/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import NewsPost from './partials/NewsPost.vue'

export default {
    name: 'OurNews',
    components: {
        // HelloWorld
        NewsPost
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    div {
        height: 10vh;
        width: 100%;
        border: 2px solid magenta;
    }
</style>