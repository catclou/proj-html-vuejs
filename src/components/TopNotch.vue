<template>
    <div class="container-fluid d-flex flex-column p-5">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto">
            
            <!-- text container  -->
            <div class="d-flex flex-column align-items-center">
                <h2 class="fw-bold w_custom m-5 text-white">See Our Top Notch Services</h2>
                <p class="lead text-white w_custom mb-5">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- cards container -->
            <div class="d-flex justify-content-center mb-5">
                <TopNotchCard v-for="info in informazioniCard" :key="info" :icon="info.icon" :heading="info.heading" :paragraph="info.paragraph" :href="info.href" class="m-2 col-2 text-white"/>
            </div>

        </div>
    </div>
</template>

<script>

import TopNotchCard from './partials/TopNotchCard.vue'

export default {
    name: 'TopNotch',
    data() {
        return {
            informazioniCard: [
                {
                    icon: 'fa-brands fa-google p-4 fa-2xl',
                    heading: 'Google SEO',
                    paragraph: 'Vestibulum in lacinia metus. Susoendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.',
                    href: '#'
                },
                {
                    icon: 'fa-solid fa-gear p-4 fa-2xl',
                    heading: 'Brand Strategy',
                    paragraph: 'Vestibulum in lacinia metus. Susoendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.',
                    href: '#'
                },
                {
                    icon: 'fa-solid fa-building p-4 fa-2xl',
                    heading: 'Local SEO',
                    paragraph: 'Vestibulum in lacinia metus. Susoendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.',
                    href: '#'
                },
                {
                    icon: 'fa-solid fa-chart-column p-4 fa-2xl',
                    heading: 'SEO Analysis',
                    paragraph: 'Vestibulum in lacinia metus. Susoendisse in enim ipsum. Nulla facilisi. Donec ante turpis, dictum sed magna et, dapibus faucibus odio.',
                    href: '#'
                }
            ]
        }
    },
    components: {
        TopNotchCard
    }
}
</script>

<style scoped lang="scss">

    .container-fluid {
        background-color: #051642;
        background-image: url('../assets/img/pattern_background.png');
        background-size: cover;

        .w_custom {
            width: 35%;
        }

    }
    
</style>