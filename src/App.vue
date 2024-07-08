<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue'
import AppListBox from './components/AppListBox.vue';
import AppShopInfo from './components/AppShopInfo.vue';




export default {
  name: "App",
  components: {
    AppHeader,
    AppListBox,
    AppShopInfo,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <div class="jumbodron">
      <div>
        <button class="target">Currents Series</button>
      </div>
    </div>
    <AppListBox />
    <AppShopInfo />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use'./styles/general.scss' as *;

main {
  background-color: black;

  .jumbodron {
    background-image: url(../src/assets/jumbotron.jpg);
    background-size: cover;
    height: 50vh;


    div {
      width: 80%;
      height: 100%;
      margin: 0 auto;
      position: relative;


      .target {
        color: white;
        padding: 10px;
        border: 1px solid blue;
        background-color: blue;
        position: absolute;
        bottom: -20px;
        text-transform: uppercase;
      }
    }
  }
}
</style>
