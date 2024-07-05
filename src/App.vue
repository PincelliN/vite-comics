<script>
import AppFooter from './components/AppFooter.vue';
import AppHeader from './components/AppHeader.vue'
import AppListBox from './components/AppListBox.vue';
import AppShopInfo from './components/AppShopInfo.vue';


export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppListBox,
    AppShopInfo
  }
}
</script>

<template>
  <AppHeader />
  <main>
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
