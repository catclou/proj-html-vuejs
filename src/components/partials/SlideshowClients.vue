<template>
    <div class="d-flex flex-column align-items-center">

        <!-- carosello -->
        <div class="slider-container mb-4 ms-2 d-flex flex-column justify-content-center align-items-center">
            <img class="rounded-circle" :src="immagini[numeroImmagine]" alt="">
            <p class="lead fst-italic text-secondary m-4 w-50">Ability proceeds from a fusion of skills, knowledge, understanding and imagination, consolidated by experience.</p>
            <div class="d-flex">
                <span class="fw-bold lead">Luis Desalvo</span>
                <span class="text-capitalize lead">, creo tech</span>
            </div>
        </div>

        <hr class="w-75 text-secondary">

    </div>


</template>

<script>

export default {
    name: 'SlideshowClients',
    data () {
        return {
            numeroImmagine: 0,
            immagini: [
                require('../../assets/img/testimonials-1.jpg'),
                require('../../assets/img/testimonials-2.jpg')
            ],
        }
    },
    created() {
            setInterval(() => {
                this.fotoSuccessiva();
            }, 3000);
        },
        methods: {
            fotoPrecedente() {
                this.numeroImmagine -= 1;
                if (this.numeroImmagine < 0)  this.numeroImmagine = (this.immagini.length - 1);
            },
            fotoSuccessiva() {
                this.numeroImmagine += 1;
                if (this.numeroImmagine > (this.immagini.length - 1)) this.numeroImmagine = 0;
            }
        }
}
</script>

<style scoped lang="scss">
    
</style>