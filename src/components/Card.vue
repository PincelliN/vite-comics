<script>
export default {
    name: "Card",
    props: {
        img: String,
        Title: String
    }
}
</script>


<template>
    <div class="Card">
        <img :src="img" :alt="Title">
        <h5>{{ Title }}</h5>
    </div>
</template>


<style lang="scss" scoped>
@use'/src/styles/partials/variables' as*;

.Card {
    flex-basis: calc((100% / 6) - 10px);
    color: $fourth-color;
    margin: 5px;

    img {
        width: 100%;
        aspect-ratio: 1 / 1.3;
    }

    h5 {
        text-align: center;
    }
}
</style>