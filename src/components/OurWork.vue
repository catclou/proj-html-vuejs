<template>
    <div class="container-fluid d-flex flex-column p-5">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto">

            <!-- text container  -->
            <div class="d-flex flex-column align-items-center m-3">
                <h2 class="fw-bold w_custom">Our Work</h2>
                <p class="lead text-secondary w_custom">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- cards container -->
            <div class="d-flex justify-content-center flex-wrap">
                <OurWorkImg v-for="info in informazioniCard" :key="info" :path="info.path" class="m-1 col-3"/>
            </div>

            <!-- button  -->
            <button class="btn btn-sm rounded-pill text-uppercase text-white mt-5">view our work</button>

        </div>
    </div>
</template>

<script>

import OurWorkImg from './partials/OurWorkImg.vue'

export default {
    name: 'OurWork',
    data() {
    return {
        informazioniCard: [
            {
                path: 'study-gallery-3-1.jpg'
            },
            {
                path: 'study-gallery-2.jpg'
            },
            {
                path: 'study-gallery-1-1.jpg'
            },
            {
                path: 'study-gallery-4-1.jpg'
            },
            {
                path: 'study-gallery-5-1.jpg'
            },
            {
                path: 'study-gallery-6-1.jpg'
            }
        ]
    }
    },
    components: {
        OurWorkImg
    }
}
</script>

<style scoped lang="scss">

    .container-fluid {
        background-color: #f7f8fa;

        .w_custom {
            width: 35%;
        }

        button {
            width: 150px;
            height: 40px;
            padding: 4px!important;
            font-size: 0.8rem;
            font-weight: 600;
            background-color: #ffa837!important;
        }

    }

</style>