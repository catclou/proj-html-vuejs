<template>
    <header class="d-flex justify-content-between">

        <!-- logo -->
        <img src="../assets/img/logo_seo_w_1x.png" alt="">

        <!-- navbar -->
        <nav class="h-100">
            <ul class="list-unstyled d-flex h-100">
                <a href="#" id="home" class="ms-3 text-capitalize list-group-item">home</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-white">who we are</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-white">what we do</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-white">Where We Work</a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-white">Careers <button class="text-uppercase btn btn-outline-warning btn-sm rounded ms-1">apply</button></a>
                <a href="#" class="ms-2 text-capitalize list-group-item text-white">news</a>
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
        height: 5vh;
        width: 70%;
        align-self: center;
        margin: 10px;
        padding-top: 5px;
        font-weight: 600;

        img {
            height: 40px;
            z-index: 1;
        }

        .list-group-item {
            border: none!important;
            background-color: transparent;
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
            z-index: 1;
        }

        .btn-group-sm > .btn, .btn-sm {
            font-size:0.6rem;
        }
    }
</style>
