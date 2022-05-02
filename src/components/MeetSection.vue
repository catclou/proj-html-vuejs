<template>
    <div class="container-fluid d-flex flex-column">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto">

            <!-- text container  -->
            <div class="d-flex flex-column align-items-center">
                <h2 class="fw-bold w_custom m-5">Meet The New Agency SEO Template From The Avada Team</h2>
                <p class="lead text-secondary w_custom mb-5">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- cards container -->
            <div class="d-flex justify-content-center">
                <MeetCard v-for="info in informazioniCard" :key="info" :icon="info.icon" :heading="info.heading" :paragraph="info.paragraph" class="m-2 col-3"/>
            </div>

            <!-- image on the bottom  -->
            <img class="w-75" src="../assets/img/agency-seo-desk-front-1200x570.jpg" alt="a desk">

        </div>
    </div>
</template>

<script>
import MeetCard from './partials/MeetCard.vue'

export default {
    name: 'MeetSection',
    data() {
        return {
            informazioniCard: [
                {
                    icon: 'fa-solid fa-road p-4 fa-2xl',
                    heading: 'Establish Goals',
                    paragraph: 'Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.'
                },
                {
                    icon: 'fa-solid fa-video p-4 fa-2xl',
                    heading: 'Work With a Team',
                    paragraph: 'Cras semper auctor aliquam. Sed porta sed lacus sit amet consectetur. Lorem ipsum dolor sit amer, consectetur adipiscin.'
                },
                {
                    icon: 'fa-solid fa-droplet p-4 fa-2xl',
                    heading: 'Get Results',
                    paragraph: 'Vestibulum scelerisque egestas lectus sit amet molestie. Donec consectetur cursus est sed blandit. Nunc sed risus lacus.'
                }
            ]
        }
    },
    components: {
        MeetCard
    }
}
</script>

<style scoped lang="scss">

    .container-fluid {
        background-color: #f8f8f8;

        .w_custom {
            width: 35%;
        }

    }
</style>