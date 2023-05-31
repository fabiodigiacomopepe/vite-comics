<script>
export default {
    name: "AppMain",
}
</script>

<template>
    <section>
        <div class="container">
            <div class="text">
                --&#62; Content goes here &#60;--
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;

section {
    background-color: #1c1c1c;
    height: 120px;
    font-weight: bold;

    .container {
        display: flex;
        width: 80%;
        margin: 0 auto;
        align-items: center;
        color: white;
        min-height: 100%;

        .text {
            font-size: 30px;
        }
    }
}
</style>
