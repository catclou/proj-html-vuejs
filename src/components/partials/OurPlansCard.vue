<template>
    <div class="d-flex flex-column p-5 pt-1 pb-4 align-items-center justify-content-center">
        <h4 class="fw-bold p-4 pt-1 pb-1 m-5 mb-4 mt-3">{{plan}}</h4>
        <div class="m-4 mt-1 d-flex align-items-center">
            <span class="align-self-start">$</span>
            <h4 class="fw-bold indaco_cust">{{price}}</h4>
            <div class="d-flex flex-column align-self-start align-items-start justify-content-center h-75">
                <span class="indaco_cust">99</span>
                <span class="fst-italic text-secondary">monthly</span>
            </div>
        </div>
        <p class="text-secondary">{{projects}} Projects</p>
        <p class="text-secondary">{{storage}} Storage</p>
        <p class="text-secondary">{{users}}</p>
        <button :class="button">start today</button>
    </div>
</template>

<script>

export default {
    name: 'OurPlansCard',
    props: {
            plan: String,
            price: String,
            projects: String,
            storage: String,
            users: String,
            button: String
    }
}
</script>

<style scoped lang="scss">
    div {
        background-color: white;
        color: black!important;

        button {
            width: 150px;
            height: 40px;
            padding: 4px!important;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .orange_cust {
            background-color: #ffa837!important;
        }

        .indaco_cust {
            color: #5f7afd!important;
        }
    }
</style>