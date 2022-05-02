<template>
    <div class="container-fluid d-flex flex-column p-5">
        <div class="row d-flex flex-column align-items-center justify-content-between mx-auto">

            <!-- text container  -->
            <div class="d-flex flex-column align-items-center m-3">
                <h2 class="fw-bold w_custom">Our News</h2>
                <p class="lead text-secondary w_custom">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium.</p>
            </div>

            <!-- cards container -->
            <div class="d-flex justify-content-center flex-wrap">
                <NewsPost v-for="info in informazioniCard" :key="info" :path="info.path" :postTitle="info.postTitle" :postLink="info.postLink" :date="info.date" :postSubtitle="info.postSubtitle" class="m-1 col-3"/>
            </div>

            <!-- button  -->
            <button class="btn btn-sm rounded-pill text-uppercase text-white mt-5">go to news</button>

        </div>
    </div>
</template>

<script>

import NewsPost from './partials/NewsPost.vue'

export default {
    name: 'OurNews',
    data() {
    return {
        informazioniCard: [
            {
                path: 'related-service-2-700x441.jpg',
                postTitle: 'why do you need a SEO agency now',
                postLink: '#',
                date: 'November 1st, 2017',
                postSubtitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit'
            },
            {
                path: 'related-service-4-700x441.jpg',
                postTitle: 'SEO tips for your startup',
                postLink: '#',
                date: 'November 1st, 2017',
                postSubtitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit'
            },
            {
                path: 'blog-post-6-700x441.jpg',
                postTitle: 'image optimization for your site',
                postLink: '#',
                date: 'November 1st, 2017',
                postSubtitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. In et scelerisque sem. Nunc molestie neque augue, at gravida mi blandit'
            }
        ]
    }
    },
    components: {
        NewsPost
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