<script>
export default {
  name: "AppHeader",
  data() {
    return {
      links: [{
        text: "characters",
        url: "#",
        state: false,
      },
      {
        text: "comics",
        url: "#",
        state: true,
      },
      {
        text: "movies",
        url: "#",
        state: false,
      },
      {
        text: "tv",
        url: "#",
        state: false,
      },
      {
        text: "games",
        url: "#",
        state: false,
      },
      {
        text: "collectibles",
        url: "#",
        state: false,
      },
      {
        text: "videos",
        url: "#",
        state: false,
      },
      {
        text: "fans",
        url: "#",
        state: false,
      },
      {
        text: "news",
        url: "#",
        state: false,
      },
      {
        text: "shop",
        url: "#",
        state: false,
      },
      ]
    }
  }
}

</script>

<template>
  <div>
    <img src="../assets/dc-logo.png" alt="">
    <nav>
      <ul>
        <li v-for="link in links" :class="link.state === true ? 'active' : ''">
          <a :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
@use'/src/styles/partials/variables' as*;

div {

  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: 0 auto;
  padding: 20px;

  img {
    width: 50px;
  }

  ul {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    text-transform: uppercase;
    font-size: 0.6rem;
    font-weight: bolder;


    li {

      padding: 15px 8px;
      color: $first-color;
    }

    .active {
      border-bottom: 3px solid $third-color;
      color: $third-color;
    }
  }
}
</style>
