<template>
    <!-- hero -->
    <div id="hero" class="container-fluid d-flex align-middle">

        <!-- text and button container -->
        <div class="row d-flex w-100">
            <div class="col-4 align_middle m_custom d-flex flex-column justify-content-between">

                <!-- title -->
                <h1 class="w-100 text-light text-start">SEM Campaigns Made Simple With Avada</h1>

                <!-- paragraph -->
                <p class="text-start text-light fs-5 mt-4 mb-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus eu ornare erat. Curabitur pulvinar elit.</p>
                
                <!-- buttons -->
                <div class="d-flex">
                    <button id="buy" class="btn btn-sm rounded-pill text-uppercase text-white">buy avada now</button>
                    <button id="contact" class="btn btn-sm rounded-pill ms-3 text-uppercase text-white">contact us</button>
                </div>
            
            </div>
        </div>
        
    </div>
</template>

<script>

export default {
    name: 'HeroFirst'
}
</script>

<style scoped lang="scss">

#hero {
        height: 75vh;
        margin-top: -7.2vh;
        background-image: url('../assets/img/1-hero-image.png');
        background-size: cover;

        .align_middle {
            align-self: center;
        }

        .m_custom {
            margin-left: 18vw;
        }

        h1 {
            font-size: 3rem;
            font-weight: bold;
        }

        button {
            width: 150px;
            height: 40px;
            padding: 4px!important;
            font-size: 0.8rem;
            font-weight: 600;
        }

        #buy {
            background-color: #ffa837!important;
        }

        #contact {
            background-color: #556eed!important;
        }
    }
</style>
