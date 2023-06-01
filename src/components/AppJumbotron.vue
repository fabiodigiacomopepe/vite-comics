<script>
export default {
    name: "AppJumbotron",
}
</script>

<template>
    <section>
        <img src="../assets/img/jumbotron.jpg" alt="jumbtron">
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

section {
    height: 320px;
}

img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
}
</style>
