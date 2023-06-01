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
            <div class="current_series">CURRENT SERIES</div>
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
        width: 75%;
        margin: 0 auto;
        color: white;
        padding: 0 0 25px 0;

        .current_series {
            background-color: $colore_primario;
            width: 200px;
            padding: 10px;
            position: relative;
            text-align: center;
            bottom: 20px;
            right: 20px;
            font-size: 24px;
        }

        .button_loadmore {
            padding: 10px 70px;
            background-color: $colore_primario;
            width: 220px;
            text-align: center;
            margin: 25px auto 0;
        }
    }
}
</style>
