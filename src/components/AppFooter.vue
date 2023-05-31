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
            <div>

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
    height: 300px;
    color: white;
    display: flex;
    justify-content: space-between;
}

img {
    height: 100%;
    width: 430px;
    object-fit: cover;
}
</style>
