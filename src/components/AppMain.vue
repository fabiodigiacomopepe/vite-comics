<script>
import AppListProducts from './AppListProducts.vue'

export default {
    name: "AppMain",
    components: {
        AppListProducts,
    }
}
</script>

<template>
    <main>
        <div class="container">
            <div class="current_series">
                <div>CURRENT SERIES</div>
            </div>
            <AppListProducts />
            <div class="button_loadmore">LOAD MORE</div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
    background-color: #1c1c1c;
    font-weight: bold;

    .container {
        @include flex_container;
        flex-wrap: wrap;
        justify-content: center;
        color: white;
        gap: 20px;
        padding: 0 0 30px 0;

        .current_series {
            width: 100%;

            div {
                background-color: $colore_primario;
                width: 200px;
                padding: 10px;
                position: relative;
                text-align: center;
                bottom: 15px;
                font-size: 24px;
            }
        }

        .button_loadmore {
            padding: 10px 70px;
            background-color: $colore_primario;
        }
    }
}
</style>
