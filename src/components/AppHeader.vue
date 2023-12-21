<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
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
                <li v-for="link in links">
                    <a :href="link.url" :class="link.current ? 'active' : ''">
                        {{ link.text }}
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
