<template>
    <a href="#" :class="aspetto">{{listItem}}</a>
</template>

<script>

export default {
    name: 'LiNavFooter',
    props: {
            listItem: String,
            aspetto: String
    }
}
</script>

<style scoped lang="scss">

    a {
        border: none;
    }

    a:hover, i:hover, .home {
            color: #ffa837!important;
    }

</style>