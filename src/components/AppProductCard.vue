<script>
export default {
    name: "AppProductCard",
    props: {
        details: Object
    }
}
</script>

<template>
    <div>
        <img :src="details.thumb" :alt="details.series">
    </div>
    <h4>{{ details.series.toUpperCase() }}</h4>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

div {
    height: 160px;
    margin-bottom: 10px;

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
    }
}

h4 {
    font-weight: 200;
    font-size: 12px;
    min-height: 30px;
}
</style>

