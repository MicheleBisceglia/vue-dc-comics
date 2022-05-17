<template>
  <header>
    <div>
      <div class="logo-container">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
    </div>
    <div>
      <ul class="header-list">
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
        <li>item</li>
      </ul>
    </div>
    <div class="header-bottom"></div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss">
header {
  height: 100px;
  width: 100%;
  display: flex;
  position: fixed;
  z-index: 999;
  background-color: white;
}
.logo-container img {
  margin-left: 150px;
  height: 70px;
  width: 70px;
  margin-top: 15px;
}
.header-list {
  margin-left: 400px;
}
.header-list li {
  list-style: none;
  display: inline;
  margin-left: 20px;
  line-height: 100px;
}
</style>
