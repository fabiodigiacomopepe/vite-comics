<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <section>
        <div class="container_blue">

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

    <section>
        <div class="container-follow_us">

        </div>
    </section>
</template>

<style scoped>
.container_blue {
    background-color: #0282f9;
    height: 130px;
}

.link_section {
    background-image: url("../src/assets/img/footer-bg.jpg");
}

.container-link {
    width: 80%;
    margin: 0 auto;
    height: 400px;
    color: white;
    display: flex;
    justify-content: space-between;
}

img {
    height: 100%;
    width: 550px;
    object-fit: cover;
}

.container-follow_us {
    background-color: #303030;
    height: 90px;
}

li {
    list-style-type: none;
    color: #767575;
    font-size: 15px;
}

.container_ul {
    display: flex;
    flex-wrap: wrap;
    width: 55%;
    padding: 40px 0;
}

h2 {
    margin-bottom: 10px;
}

ul {
    line-height: 1.3;
    margin-bottom: 30px;
}

.col_left {
    width: 35%;
}

.col_right {
    width: 65%;
    display: flex;
    gap: 50px;
}
</style>
