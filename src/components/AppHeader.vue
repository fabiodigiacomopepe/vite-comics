<script>
export default {
    name: "AppHeader",
    data() {
        return {
            percorsoLogo: "./src/assets/img/dc-logo.png"
        }
    },
    props: {
        sezioniNav: Array
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div>
                <a href="#">
                    <img :src="percorsoLogo" alt="logo">
                </a>
            </div>

            <nav>
                <ul>
                    <li v-for="(sezione, index) in sezioniNav" :key="index">
                        <a :href="sezione.url" :class="sezione.current ? 'active' : ''">
                            {{ sezione.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

.container {
    @include flex_container;
    justify-content: space-between;
    font-weight: bold;

    img {
        width: 65px;
        max-width: 100%;
    }

    ul {
        display: flex;
        gap: 25px;

        li {
            font-size: 12px;

            a {
                color: #646664;
                height: 100%;
                display: inline-block;
                line-height: 85px;
            }
        }
    }

    .active {
        color: $colore_primario;
        border-bottom: 3px solid $colore_primario;
    }
}
</style>

