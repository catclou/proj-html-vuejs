<template>
    <div class="d-flex flex-column p-4 align-items-center justify-content-center">
        <i :class="icon"></i>
        <h3 class="fw-bold m-4">{{heading}}</h3>
        <p class="w-75">{{paragraph}}</p>
    </div>
</template>

<script>

export default {
    name: 'MeetCard',
    props: {
            icon: String,
            heading: String,
            paragraph: String
    }
}
</script>

<style scoped lang="scss">

    div {
        background-color: white;

        i {
            color: #ffa837;
        }
    }
</style>