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
        <img :src="img" alt="">
        <h5>{{ Title }}</h5>
    </div>

</template>


<style lang="scss" scoped>
.Card {
    flex-basis: calc((100% / 6) - 5px);
    color: white;

    img {
        width: 100%;
        object-fit: cover;
    }

    h5 {
        text-align: center;
    }
}
</style>