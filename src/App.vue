<script>
import "@fontsource/roboto";
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue'
import AppJumbodron from './components/AppJumbodron.vue';
import AppListBox from './components/AppListBox.vue';
import AppShopInfo from './components/AppShopInfo.vue';




export default {
  name: "App",
  components: {
    AppHeader,
    AppListBox,
    AppJumbodron,
    AppShopInfo,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <AppJumbodron />
    <AppListBox />
    <AppShopInfo />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use'./styles/general.scss' as *;


main {
  background-color: black;
}
</style>
