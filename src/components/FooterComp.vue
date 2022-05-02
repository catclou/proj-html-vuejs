<template>
    <div class="p-3">
        <img src="../assets/img/logo_seo_1x.png" class="m-3" alt="">
        <nav>
            <ul class="list-unstyled d-flex h-100 d-flex justify-content-center m-4">
                <a href="#" id="home" class="ms-3 text-capitalize list-group-item text-secondary">home</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">who we are</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">what we do</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">Where We Work</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">Careers</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">news</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-secondary">get in touch now</a>
            </ul>
        </nav>
        <p class="text-secondary">Copyright 2012 - 2020 | Avada Theme by <a href="#" class="fw-bold text-decoration-none text-secondary">ThemeFusion</a> | All Rights Reserved | Powered by <a href="#" class="fw-bold text-decoration-none text-secondary">WordPress</a></p>
        <div class="d-flex justify-content-center">
            <a href="#">
                <i class="fa-brands fa-facebook-f p-2 text-secondary"></i>
            </a>
            <a href="#">
                <i class="fa-brands fa-instagram p-2 text-secondary"></i>
            </a> 
            <a href="#">
                <i class="fa-brands fa-twitter p-2 text-secondary"></i>
            </a> 
            <a href="#">
                <i class="fa-brands fa-youtube p-2 text-secondary"></i>
            </a> 
        </div>
        <!-- <LiNavFooter/> -->
        <!-- <SocialIcons/> -->
    </div>
</template>

<script>
// import "bootstrap"
// import HelloWorld from './components/HelloWorld.vue'
// import LiNavFooter from './partials/LiNavFooter.vue'
// import SocialIcons from './partials/SocialIcons.vue'

export default {
    name: 'FooterComp',
    components: {
        // HelloWorld
        // LiNavFooter,
        // SocialIcons
    }
}
</script>

<style scoped lang="scss">
// @import "bootstrap/dist/css/bootstrap.min.css";
    a {
        border: none;
    }

    a:hover, i:hover, #home {
            color: #ffa837!important;
        }
</style>