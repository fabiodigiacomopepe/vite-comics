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
                    <a :href="sezione.url" :class="sezione.current ? 'active' : ''">
                        {{ sezione.text }}
                    </a>
                </li>
            </ul>
        </div>
    </section>
</template>

<style scoped>
a {
    text-decoration: none;
    color: #646664;
    height: 100%;
    display: inline-block;
    line-height: 85px;
}

.container {
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: 0 auto;
    align-items: center;
    font-weight: bold;
}

img {
    width: 65px;
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

.active {
    color: #0282f9;
    border-bottom: 3px solid #0282f9;
}
</style>

