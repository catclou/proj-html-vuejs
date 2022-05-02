<template>
    <div class="d-flex flex-column p-4 align-items-center justify-content-center">
        <img :src="require('../../assets/img/' + path)" alt="" class="w-100">
    </div>
</template>

<script>


export default {
    name: 'OurWorkImg',
    props: {
        path: String
    }
}
</script>

<style scoped lang="scss">

</style>
