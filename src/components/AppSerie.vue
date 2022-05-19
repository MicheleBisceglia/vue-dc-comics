<template>
  <div class="list">
    <img :src="comicsObj.thumb" alt="" />
    <h4>{{ comicsObj.series }}</h4>
  </div>
</template>

<script>
import SerieList from "./SerieList.vue";
export default {
  name: "AppSerie",
  components: {
      SerieList
  },
  props: {
    comicsObj: Object,
  },
};
</script>

<style lang="scss" scoped>
.list {
    width: calc(100% / 6);
    text-align: center;
    color: white;
    font-size: 70%;
}
.list img {
    height: 70%;
    width: 70%;
}
</style>