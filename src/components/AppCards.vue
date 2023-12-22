<script>
export default {
    props: {
        details: Object
    },
    name: "AppCards",
}
</script>

<template>
    <div class="prod-card">
        <img :src="details.thumb" alt="img">
        <h3>{{ details.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;



.prod-card {
    background-color: white;
    border: 2px solid black;
    display: inline-block;
    width: calc((100% / 6) - 10px);
    margin: 5px;

    h3 {
        color: $primary;
        font-size: 12px;
    }

    img {
        width: 100%;
        height: 80%;
    }
}
</style>