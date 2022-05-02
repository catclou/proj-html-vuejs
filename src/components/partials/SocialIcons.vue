<template>
    <a :href="href">
        <i :class="icon"></i>
    </a>
</template>

<script>

export default {
    name: 'SocialIcons',
    props: {
            icon: String,
            href: String
    }
}
</script>

<style scoped lang="scss">

    a:hover, i:hover {
        color: #ffa837!important;
    }
    
</style>