<script >
export default{
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
      <li v-for="link in links"
      :class="link.state ? 'active':''">
        <a :href="link.url">{{link.text}}</a>
      </li>
      
    </ul>
  </nav>
  </div>
</template>

<style scoped>
  div{
   
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
  ul{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    list-style: none;
  }
  li{
    margin: 1rem;
  }
  .active{
    border-bottom: 3px solid blue;
  }
</style>
