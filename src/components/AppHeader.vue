<template>
  <header>
    <div>
      <div class="logo-container">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
    </div>
    <div>
      <ul class="header-list">
        <li
          v-for="(item, index) in links"
          :key="index"
          :class="{ active: item.active }"
        >
          <a>{{ item.text }}</a>
        </li>
      </ul>
    </div>
    <div class="header-bottom"></div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      links: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: true,
        },
        {
          url: "#",
          text: "Movies",
          active: false,
        },
        {
          url: "#",
          text: "TV",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Video",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "news",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/common.scss";

header {
  height: 100px;
  width: 100%;
  display: flex;
  position: fixed;
  z-index: 999;
  background-color: white;
  min-width: 900px;
}
.logo-container img {
  margin-left: 150px;
  height: 70px;
  width: 70px;
  margin-top: 15px;
}
.header-list {
  margin-left: 300px;
}
.header-list li {
  display: inline;
  margin-left: 10px;
  text-transform: uppercase;
  font-size: 70%;
  line-height: 100px;

  &.active {
    border-bottom: solid #0282f9 5px;
  }
}
</style>
