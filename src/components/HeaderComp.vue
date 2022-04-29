<template>
    <header class="d-flex justify-content-between">
        <img src="../assets/img/logo_seo_1x.png" alt="">
        <nav class="h-100">
            <ul class="list-unstyled d-flex h-100">
                <a href="#" id="home" class="ms-3 text-capitalize list-group-item">home</a>
                <a href="#" class="ms-3 text-capitalize list-group-item">who we are</a>
                <a href="#" class="ms-3 text-capitalize list-group-item">what we do</a>
                <a href="#" class="ms-3 text-capitalize list-group-item">Where We Work</a>
                <a href="#" class="ms-3 text-capitalize list-group-item">Careers <button class="text-uppercase btn btn-outline-warning btn-sm rounded ms-1">apply</button></a>
                <a href="#" class="ms-3 text-capitalize list-group-item">news</a>
                <button id="get_in_touch" class="btn btn-warning btn-sm rounded-pill ms-3 text-uppercase text-white">get in touch now</button>
            </ul>
        </nav>
    </header>
</template>

<script>

export default {
    name: 'HeaderComp',
}
</script>

<style scoped lang="scss">
    header {
        height: 10vh;
        width: 70%;
        align-self: center;
        margin: 10px;
        font-weight: 600;

        img {
            height: 40px;
        }

        .list-group-item {
            border: none!important;
        }

        a:hover, #home {
            color: #ffa837!important;
        }

        #get_in_touch {
            width: 150px;
            height: 40px;
            padding: 4px!important;
            font-size: 0.8rem;
            font-weight: 600;
            background-color: #ffa837!important;
        }

        .btn-group-sm > .btn, .btn-sm {
            font-size:0.6rem;
        }
    }
</style>
