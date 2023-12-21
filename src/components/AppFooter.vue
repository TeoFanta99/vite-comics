<script>
export default {
    name: "AppFooter",
    data() {
        return {
            dcComicsLinks: [
                {
                    text: "Characters",
                    url: "#",
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "TV",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
            ],
            shopLinks: [
                {
                    text: "Shop DC",
                    url: "#",
                },
                {
                    text: "Shop DC Collectibles",
                    url: "#",
                },
            ],
            dcLinks: [
                {
                    text: "Terms Of Use",
                    url: "#",
                },
                {
                    text: "Privacy policy (New)",
                    url: "#",
                },
                {
                    text: "Ad Choices",
                    url: "#",
                },
                {
                    text: "Advertising",
                    url: "#",
                },
                {
                    text: "Jobs",
                    url: "#",
                },
                {
                    text: "Subscriptions",
                    url: "#",
                },
                {
                    text: "Talent Workshops",
                    url: "#",
                },
                {
                    text: "CPSC Certificates",
                    url: "#",
                },
                {
                    text: "Ratings",
                    url: "#",
                },
                {
                    text: "Shop Help",
                    url: "#",
                },
                {
                    text: "Contact Us",
                    url: "#",
                }
            ],
            sitesLinks: [
                {
                    text: "DC",
                    url: "#",
                },
                {
                    text: "MAD Magazine",
                    url: "#",
                },
                {
                    text: "DC Kids",
                    url: "#",
                },
                {
                    text: "DC Universe",
                    url: "#",
                },
                {
                    text: "DC Power Visa",
                    url: "#",
                },
            ]
        }
    }
}
</script>

<template>
    <div class="top-footer">
        <!-- questa è la parte con le 5 icone -->
    </div>
    <div class="link-section">
        <!-- parte del footer coi vari link -->
        <div class="link-container">

            <div class="col">
                <span>DC COMICS</span>
                <ul>
                    <li v-for="link in dcComicsLinks">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul> <br>
                <span>SHOP</span>
                <ul>
                    <li v-for="link in shopLinks">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="col">
                <span>DC</span>
                <ul>
                    <li v-for="link in dcLinks">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="col">
                <span>SITES</span>
                <ul>
                    <li v-for="link in sitesLinks">
                        <a :href="link.url">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </div>

    </div>
    <div class="bottom-footer">
        <!-- parte più in fondo del footer -->
        <button type="button">SIGN-UP NOW!</button>
        <div>
            <span>FOLLOW US</span>
            <!-- inserire icone di facebook, twitter, yt e pinterest -->
        </div>
    </div>
</template>


<style lang="scss" scoped>
.top-footer {
    background-color: #0882F9;
    min-height: 100px;
}

.link-section {
    background-image: url(../assets/img/footer-bg.jpg);
    height: 350px;
    padding-top: 40px;
    display: flex;
}

.link-container {
    display: flex;
    width: 35%;
    margin-left: 150px;

    .col {
        width: calc(100% / 3);

        span {
            color: white;
            font-size: 18px;
        }

        ul {
            list-style-type: none;
            margin-top: 10px;

            a {
                text-decoration: none;
                font-size: 12px;
                color: #959595;

                &:hover {
                    background-color: azure;
                }
            }
        }
    }
}

.bottom-footer {
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-color: #303030;
    // debug
    min-height: 100px;

    button {
        background: none;
        border: 2px solid #0882F9;
        padding: 10px;
        color: white;
    }

    span {
        color: #0882F9;
    }
}
</style>
