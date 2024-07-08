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
        <div>
            <img :src="img" alt="">
        </div>

        <h5>{{ Title }}</h5>
    </div>

</template>


<style lang="scss" scoped>
.Card {
    flex-basis: calc((100% / 6) - 10px);

    color: white;
    margin: 5px;

    div {
        object-fit: cover;

        img {
            width: 100%;
            height: 100%;
        }
    }

    h5 {
        text-align: center;
    }
}
</style>