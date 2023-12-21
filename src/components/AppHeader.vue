<script>
export default {
    name: "AppHeader",
}
</script>

<template>
    <header>
        <a href="/" class="brand">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </a>

        <!-- navigazione menù principale -->
        <nav>
            <ul>
                <li>
                    <a href="" class="active">
                        testo
                    </a>
                </li>
                <li>
                    <a href="" class="">
                        testo
                    </a>
                </li>
            </ul>
        </nav>


    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    text-align: center;
    display: flex;
    justify-content: space-evenly;
    margin-top: 20px;

    ul {
        list-style: none;
        margin: 2.5rem 1rem 4rem;
        @include center ();

        li a {
            display: inline-block;
            padding: 1rem;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.3s;

            &.active,
            &:hover {
                background: lighten($primary, 70%);
            }
        }
    }
}
</style>
