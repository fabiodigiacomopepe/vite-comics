<script>
import AppProductCard from './AppProductCard.vue'

export default {
    name: "AppListProducts",
    components: {
        AppProductCard
    },
    data() {
        return {
            products: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://dope.tw/wp-content/uploads/2022/11/LFP11605P.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/51Cj4Djz88L.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/I/71Dp96zXS+L.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/P/B08HB1NV81.01._SCLZZZZZZZ_SX500_.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/P/B08HVW31NW.01._SCLZZZZZZZ_SX500_.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/P/B08LW3QLD7.01._SCLZZZZZZZ_SX500_.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://m.media-amazon.com/images/P/B08KHTTXSV.01._SCLZZZZZZZ_SX500_.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.mangaforever.net/wp-content/uploads/2015/03/catwoman-1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="(product, index) in products" :key="index">
            <AppProductCard :details="product" />
        </li>
    </ul>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

ul {
    width: 100%;
    display: flex;
    gap: 20px;
    flex-wrap: wrap;

    li {
        width: calc(100% / 6 - 20px);
        margin-bottom: 10px;
    }
}
</style>

