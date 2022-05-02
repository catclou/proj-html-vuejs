<template>
    <div class="container-fluid d-flex flex-column p-5">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto">

            <!-- text container  -->
            <div class="d-flex flex-column align-items-center m-3 p-5">
                <h2 class="fw-bold text-white m-2">Start Your Free Consultation</h2>
                <p class="lead text-secondary w-75 text-white">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- button  -->
            <button class="btn btn-sm rounded-pill text-uppercase text-white">contact us now</button>

        </div>
    </div>
</template>

<script>

export default {
    name: 'FreeConsultation',
    components: {
        // HelloWorld
    }
}
</script>

<style scoped lang="scss">
    .container-fluid {
        background-color: rgba(0, 0, 0, .6);
        background-image: url('../assets/img/case-study-gallery-3-1-800x600.jpg');
        background-size: cover;
        background-position-y: 40%;
        
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