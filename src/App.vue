<template>
  <div id="app">
    <AppHeader />
    <main></main>
    <AppPrefooter />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppPrefooter from "./components/AppPrefooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppPrefooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
#app {
  min-width: 900px
}
main {
  background-color: #1c1c1c;
  height: 200px;
}
</style>
