<template>
    <div class="container-fluid d-flex flex-column align-items-center p-4">
        <h2 class="fw-bold w_custom m-5 text-capitalize">what our clients say</h2>
        <SlideshowClients/>
        <div class="d-flex w-50 justify-content-between mt-2 mb-5">
            <img src="../assets/img/clients_partner_5-200x202.png" alt="">
            <img src="../assets/img/clients_partner_6-200x202.png" alt="">
            <img src="../assets/img/clients_partner_1-200x202.png" alt="">
            <img src="../assets/img/clients_partner_2-200x202.png" alt="">
        </div>

    </div>
</template>

<script>

import SlideshowClients from './partials/SlideshowClients.vue'

export default {
    name: 'OurClients',
    components: {
        SlideshowClients
    }
}
</script>

<style scoped lang="scss">
    img {
        height: 8rem;
    }
</style>