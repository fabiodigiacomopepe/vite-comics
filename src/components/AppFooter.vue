<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <section class="container_blue-section">
        <div class="container_blue">
            <div>
                <img class="b" src="src/assets/img/buy-comics-digital-comics.png" alt="buy-comics-digital-comics">
                <span>DIGITAL COMICS</span>
            </div>

            <div>
                <img class="s" src="src/assets/img/buy-comics-merchandise.png" alt="buy-comics-merchandise">
                <span>DC MERCHAINDISE</span>
            </div>

            <div>
                <img class="s" src="src/assets/img/buy-comics-subscriptions.png" alt="buy-comics-subscriptions">
                <span>SUBSCRIPTIONS</span>
            </div>

            <div>
                <img class="b" src="src/assets/img/buy-comics-shop-locator.png" alt="buy-comics-shop-locator">
                <span>COMIC SHOP LOCATOR</span>
            </div>

            <div>
                <img class="svg" src="src/assets/img/buy-dc-power-visa.svg" alt="buy-dc-power-visa">
                <span>DC POWER VISA</span>
            </div>
        </div>
    </section>

    <section class="link_section">
        <div class="container-link">
            <div class="container_ul">
                <div class="col_left">
                    <div>
                        <h2>DC COMICS</h2>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>

                    <div>
                        <h2>SHOP</h2>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>

                <div class="col_right">
                    <div>
                        <h2>DC</h2>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact US</li>
                        </ul>
                    </div>

                    <div>
                        <h2>SITES</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div>
                <img src="src/assets/img/dc-logo-bg.png" alt="logo-big">
            </div>
        </div>
    </section>

    <section class="section_followus">
        <div class="container-follow_us">
            <div class="button_signup">SIGN-UP NOW!</div>

            <div class="rightside_followus">
                <span>FOLLOW US</span>
                <img src="src/assets/img/footer-facebook.png" alt="">
                <img src="src/assets/img/footer-twitter.png" alt="">
                <img src="src/assets/img/footer-youtube.png" alt="">
                <img src="src/assets/img/footer-pinterest.png" alt="">
                <img src="src/assets/img/footer-periscope.png" alt="">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

.container_blue-section {
    background-color: $colore_primario;

    .container_blue {
        width: 80%;
        margin: 0 auto;
        height: 130px;
        color: white;
        display: flex;
        align-items: center;
        justify-content: space-around;

        div {
            display: flex;
            align-items: center;

            img.b {
                width: 30px;
            }

            img.s {
                width: 40px;
            }

            img.svg {
                width: 50px;
            }

            span {
                margin-left: 10px;
                font-size: 12px;
            }
        }
    }
}

.link_section {
    background-image: url("../src/assets/img/footer-bg.jpg");

    .container-link {
        width: 80%;
        margin: 0 auto;
        height: 400px;
        color: white;
        display: flex;
        justify-content: space-between;

        .container_ul {
            display: flex;
            flex-wrap: wrap;
            width: 55%;
            padding: 40px 0;

            .col_left {
                width: 35%;
            }

            .col_right {
                width: 65%;
                display: flex;
                gap: 50px;
            }

            h2 {
                margin-bottom: 10px;
            }

            ul {
                line-height: 1.3;
                margin-bottom: 30px;

                li {
                    color: #767575;
                    font-size: 15px;
                }
            }
        }

        img {
            height: 100%;
            width: 550px;
            object-fit: cover;
        }
    }
}

.section_followus {
    background-color: #303030;

    .container-follow_us {
        height: 90px;
        width: 80%;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;

        .button_signup {
            width: 140px;
            color: white;
            padding: 10px 20px;
            border: 2px solid $colore_primario;
        }

        .rightside_followus {
            color: $colore_primario;
            font-weight: bold;

            img {
                width: 25px;
                margin-left: 10px;
            }

            span {
                position: relative;
                bottom: 7px;
                margin-right: 10px;
            }
        }
    }
}
</style>
