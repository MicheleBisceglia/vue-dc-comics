<template>
  <div class="pre-footer">
    <div class="container">
      <ul>
        <li v-for="(item, index) in icons" :key="index">
          <img :src="require(`../assets/${item.img}`)" alt="" />
          <h3>{{ item.text }}</h3>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppPrefooter",
  data: function () {
    return {
      icons: [
        {
          img: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "DC merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "Subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "Comic shop locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "DC power visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.pre-footer {
  background-color: #0282f9;
  color: white;
  padding: 1.5rem;
  & ul {
    display: flex;
    justify-content: center;
  }
  li img {
    height: 40px;
    margin-right: 1rem;
  }
  li {
    width: calc(100% / 7);
    display: flex;
    justify-content: center;
    align-items: center;
  }
  h3 {
    font-size: 70%;
  }
}
</style>
