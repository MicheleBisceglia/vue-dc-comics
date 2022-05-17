<template>
  <header>
    <div>
      <div class="logo-container"></div>
    </div>
    <div class="header-list">
      <ul></ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss">
.logo-container {
  height: 100px;
  width: 100px;
  background-color: yellowgreen;
  float: left;
  margin-left: 100px;
}
.header-list {
  height: 100px;
  width: 300px;
  background-color: red;
  float: right;
  margin-right: 100px;
}
</style>
