<template>
    <div class="d-flex flex-column p-4 align-items-center justify-content-center">
        <img :src="require('../../assets/img/' + path)" alt="" class="w-100">
        <a :href="postLink" class="text-decoration-none fw-bold mt-3 mb-1 text-capitalize">{{postTitle}}</a>
        <span class="mb-3">{{date}}</span>
        <p class="lead">{{postSubtitle}}</p>
    </div>
</template>

<script>
export default {
    name: 'NewsPost',
    props: {
        path: String,
        postTitle: String,
        postLink: String,
        date: String,
        postSubtitle: String
    }
}
</script>

<style scoped lang="scss">
    a {
        font-size: 1.1rem!important;
        color: #ffa837!important;
    }

    span {
        font-size: 0.8rem!important;
        color: #606166;
    }

    p {
        color: #606166;
        font-size: 1rem!important;
    }
</style>