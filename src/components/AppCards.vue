<script>
export default {
    props: {
        cards: Array
    },
    name: "AppCards",
}
</script>

<template>
    <div class="prod-card">
        <img src="https://www.coverbrowser.com/image/action-comics/1-1.jpg" alt="img">
        <h3>Titolo</h3>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;



.prod-card {
    background-color: white;
    border: 2px solid black;
    display: inline-block;
    height: auto;
    width: calc((100% / 5) - 10px);
    margin: 5px;

    h3 {
        color: $primary;
    }

    img {
        width: 100%;
        height: auto;
    }
}
</style>