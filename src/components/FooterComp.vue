<template>
    <div>
        <LiNavFooter/>
        <SocialIcons/>
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
import LiNavFooter from './partials/LiNavFooter.vue'
import SocialIcons from './partials/SocialIcons.vue'

export default {
    name: 'FooterComp',
    components: {
        // HelloWorld
        LiNavFooter,
        SocialIcons
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