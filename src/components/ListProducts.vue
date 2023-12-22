<script>
import AppCards from './AppCards.vue'

export default {
    components: {
        AppCards
    },
    name: "ListProducts",
}
</script>

<template>
    <section class="products">
        <h2> Content goes here </h2>
        <AppCards />
    </section>
</template>

<style lang="scss" scoped>
.products {
    padding: 4rem 1rem;
    text-align: center;
    background-color: #000;

    h1 {
        font-weight: 600;
    }
}
</style>
