<template>
    <div class="p-3">
        <img src="../assets/img/logo_seo_1x.png" class="m-3" alt="">

        <!-- navbar  -->
        <nav>
            <ul class="list-unstyled d-flex h-100 d-flex justify-content-center m-4">
                <LiNavFooter v-for="info in informazioniCard" :key="info" :listItem="info.listItem" :aspetto="info.aspetto"/>
            </ul>
        </nav>

        <!-- signature  -->
        <p class="text-secondary">Copyright 2012 - 2020 | Avada Theme by <a href="#" class="fw-bold text-decoration-none text-secondary">ThemeFusion</a> | All Rights Reserved | Powered by <a href="#" class="fw-bold text-decoration-none text-secondary">WordPress</a></p>
        
        <!-- social  -->
        <div class="d-flex justify-content-center">
            <SocialIcons v-for="social in informazioniSocial" :key="social" :icon="social.icon" :href="social.href"/>
        </div>
    </div>
</template>

<script>
import LiNavFooter from './partials/LiNavFooter.vue'
import SocialIcons from './partials/SocialIcons.vue'

export default {
    name: 'FooterComp',
    data() {
        return {
            informazioniCard: [
                {
                    listItem: 'home',
                    aspetto: 'home ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'who we are',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'what we do',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'where we work',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'careers',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'news',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                },
                {
                    listItem: 'get in touch now',
                    aspetto: 'ms-3 text-capitalize list-group-item text-secondary border-none text-decoration-none'
                }
            ],
            informazioniSocial: [
                {
                    icon: 'fa-brands fa-facebook-f p-2 text-secondary',
                    href: '#'
                },
                {
                    icon: 'fa-brands fa-instagram p-2 text-secondary',
                    href: '#'
                },
                {
                    icon: 'fa-brands fa-twitter p-2 text-secondary',
                    href: '#'
                },
                {
                    icon: 'fa-brands fa-youtube p-2 text-secondary',
                    href: '#'
                }
            ]
        }
    },
    components: {
        LiNavFooter,
        SocialIcons
    }
}
</script>

<style scoped lang="scss">
    a {
        border: none;
    }

    a:hover, i:hover, #home {
            color: #ffa837!important;
    }
</style>