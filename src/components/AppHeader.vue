<script>
export default {
    name: "AppHeader",
    data() {
        return {
            percorsoLogo: "./src/assets/img/dc-logo.png",
            sezioniNav: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false
                },
                {
                    text: "TV",
                    url: "#",
                    current: false
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div>
                <img :src="percorsoLogo" alt="logo">
            </div>

            <ul>
                <li v-for="sezione in sezioniNav">
                    {{ sezione.text }}
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped>
.container {
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: 0 auto;
    align-items: center;
    padding: 15px 0;
    font-weight: bold;
}

img {
    width: 80px;
    max-width: 100%;
}

ul {
    display: flex;
    gap: 25px;
}

li {
    list-style-type: none;
    font-size: 12px;
}
</style>

