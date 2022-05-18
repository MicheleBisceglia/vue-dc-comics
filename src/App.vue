<template>
  <div id="app">
    <AppHeader />
    <main></main>
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";

main {
  background-color: #1c1c1c;
  height: 200px;
}
</style>
