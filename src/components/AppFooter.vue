<template>
  <footer>
    <div class="pre-footer"></div>
    <div class="footer">
      <div class="footer-list">
        <div class="col">
          <h3>Title</h3>
          <ul>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
          </ul>
          <h3>Title</h3>
          <ul>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
          </ul>
        </div>
        <div class="col">
          <h3>Title</h3>
          <ul>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
          </ul>
        </div>
        <div class="col">
          <h3>Title</h3>
          <ul>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
            <li>ciao</li>
          </ul>
        </div>
      </div>
      <div class="footer-logo"></div>
    </div>
    <div class="footer-bottom"></div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style lang="scss">
@import "../style/common.scss";

.pre-footer {
  height: 100px;
  background-color: #0282f9;
}
.footer {
  width: 100%;
  height: 300px;
  background-image: url(../assets/footer-bg.jpg);
  color: white;
  display: flex;
  flex-wrap: wrap;
  & .footer-list {
    display: flex;
    max-width: 200px;
    padding-left: 20%;
    padding-top: 50px;
    padding-right: 30%;
  }
  & .footer-logo {
    height: 100%;
    width: 400px;
    background-image: url(../assets/dc-logo-bg.png);
    background-size: contain;
    background-repeat: no-repeat;
  }
}

.footer-bottom {
  height: 70px;
  background-color: #1c1c1c;
}

.col {
  margin-left: 40px;
}
</style>
