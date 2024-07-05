<script>
export default {
  name: "AppShopInfo",
  data() {
    return {
      infos: [{
        testo: "Digital Comics",
        lin: "../assets/buy-comics-digital-comics.png",
      },
      {
        testo: "Dc Merchandise",
        lin: "../assets/buy-comics-merchandise.png",
      },
      {

        testo: "Subsciption",
        lin: "../assets/buy-comics-shop-locator.png",
      },
      {
        testo: "Comic Shop Locator",
        lin: "../assets/buy-comics-subscriptions.png",
      },
      {
        testo: "dc power visa",
        lin: "../assets/buy-dc-power-visa.svg",
      }
      ]
    }
  }
}
</script>

<template>
  <div>
    <ul>
      <li v-for="info in infos"><a href="#"><img :src="info.lin">{{ info.testo }}</a></li>

    </ul>

  </div>
</template>
<style scoped>
div {
  background-color: cornflowerblue;
  color: white;

  ul {
    margin: 0 auto;
    list-style: none;
    width: 80%;
    display: flex;
    justify-content: space-around;
  }
}
</style>