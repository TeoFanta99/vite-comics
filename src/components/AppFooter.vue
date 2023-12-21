<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <div class="top-footer">
        <!-- questa è la parte con le 5 icone -->
    </div>
    <div class="link-section">
        <!-- parte del footer coi vari link -->
        <div class="link-container">
            <div class="col"></div>
            <div class="col"></div>
            <div class="col"></div>
        </div>
    </div>
    <div class="bottom-footer">
        <!-- parte più in fondo del footer -->
    </div>
</template>

<style lang="scss" scoped>
.top-footer {
    background-color: #0882F9;
    // debug
    min-height: 100px;
}

.link-section {
    background-image: url(../assets/img/footer-bg.jpg);
    // debug
    min-height: 350px;
    padding-top: 40px;
}

.link-container {
    display: flex;
    // debug
    min-height: 250px;
    background-color: orange;
    width: 30%;
    margin-left: 150px;

    .col {
        border: 1px solid black;
        // debug
        width: calc(100% / 3);
    }
}
</style>
