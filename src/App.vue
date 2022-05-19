<template>
  <div id="app">
    <AppHeader />
    <main>
      <div class="banner"></div>
      <div class="series">
        <SerieList />
      </div>
    </main>
    <AppPrefooter />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppFooter from "./components/AppFooter.vue";
import AppPrefooter from "./components/AppPrefooter.vue";
import SerieList from "./components/SerieList.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppFooter,
    AppPrefooter,
    SerieList,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
#app {
  min-width: 900px;
}
main {
  background-color: #1c1c1c;
}
.banner {
  background-image: url(./assets/jumbotron.jpg);
  background-size: cover;
  background-position: top;
  padding-top: 350px;
}
.series {
  width: 70%;
  margin: 0 auto;
}
</style>
