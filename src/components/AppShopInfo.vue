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
        testo: "Comic Shop Locator",
        lin: "../assets/buy-comics-subscriptions.png",
      },
      {

        testo: "Subsciption",
        lin: "../assets/buy-comics-shop-locator.png",
      },
      {
        testo: "dc power visa",
        lin: "../assets/buy-dc-power-visa.svg",
      }
      ]
    };
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    }
  }
};
</script>

<template>
  <div>
    <ul>
      <li v-for="info in infos"><a href="#"><img :src="getImagePath(`${info.lin}`)"></a><span>{{ info.testo }}</span>
      </li>

    </ul>

  </div>
</template>
<style lang="scss" scoped>
@use'/src/styles/partials/variables' as*;

div {
  background-color: $second-color;
  color: $fourth-color;

  ul {
    margin: 0 auto;
    width: 80%;
    display: flex;
    justify-content: space-around;

    li {
      display: flex;
      align-items: center;
      padding: 10px;
      gap: 5px;

      img {
        width: 40px;
        aspect-ratio: 1/1;
      }

      span {
        text-transform: uppercase;
        font-size: 0.9rem;
      }

    }
  }
}
</style>