<script>
export default {
    name: "Jumbodron"
}
</script>

<template>
    <div class="jumbodron">
        <div>
            <button class="target">Currents Series</button>
        </div>
    </div>
</template>



<style lang="scss" scoped>
@use'/src/styles/partials/variables' as*;

.jumbodron {
    background-image: url(../src/assets/jumbotron.jpg);
    background-size: cover;
    height: 50vh;


    div {
        width: 80%;
        height: 100%;
        margin: 0 auto;
        position: relative;
        color: $fourth-color;

        .target {

            border: 1px solid $third-color;
            background-color: $third-color;
            position: absolute;
            bottom: -20px;
            padding: 10px;
            color: white;
            text-transform: uppercase;
        }
    }
}
</style>