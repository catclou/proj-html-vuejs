<template>
    <div class="container-fluid d-flex flex-column p-5">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto text-dark">
            
            <!-- text container  -->
            <div class="d-flex flex-column align-items-center">
                <h2 class="fw-bold w_custom m-5 text-white">Our Plans</h2>
                <p class="lead text-white w_custom mb-5">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- cards container -->
            <div class="d-flex justify-content-center mb-5">
                <OurPlansCard v-for="info in informazioniCard" :key="info" :plan="info.plan" :price="info.price" :projects="info.projects" :storage="info.storage" :users="info.users" :button="info.button" class="m-2 col-2 text-white"/>
            </div>

        </div>
    </div>
</template>

<script>
import OurPlansCard from './partials/OurPlansCard.vue'

export default {
    name: 'OurPlans',
    data() {
        return {
            informazioniCard: [
                {
                    plan: 'Standard',
                    price: '19',
                    projects: '5',
                    storage: '5 GB',
                    users: 'Unlimited users',
                    button: 'btn btn-sm btn-outline-dark rounded-pill text-uppercase mt-3'
                },
                {
                    plan: 'Premium',
                    price: '29',
                    projects: '10',
                    storage: '15 GB',
                    users: 'Unlimited users',
                    button: 'btn btn-sm btn-outline-dark rounded-pill text-uppercase mt-3'
                },
                {
                    plan: 'Professional',
                    price: '39',
                    projects: '15',
                    storage: '30 GB',
                    users: 'Unlimited users',
                    button: 'btn btn-sm orange_cust text-white rounded-pill text-uppercase mt-3'
                },
                {
                    plan: 'Extreme',
                    price: '59',
                    projects: 'Unlimited',
                    storage: 'Unlimited',
                    users: 'Unlimited users',
                    button: 'btn btn-sm btn-outline-dark rounded-pill text-uppercase mt-3'
                }
            ]
        }
    },
    components: {
        OurPlansCard
    }
}
</script>

<style scoped lang="scss">
    .container-fluid {
        background-color: #051642;
        background-image: url('../assets/img/background1.jpg');
        background-size: cover;

        .w_custom {
            width: 35%;
        }

    }
</style>