<script>
export default {
    name: "AppMain",
}
</script>

<template>
    <main>
        <div class="container">
            <div class="text">
                --&#62; Content goes here &#60;--
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
    background-color: #1c1c1c;
    height: 120px;
    font-weight: bold;

    .container {
        @include flex_container;
        color: white;
        min-height: 100%;

        .text {
            font-size: 30px;
        }
    }
}
</style>
