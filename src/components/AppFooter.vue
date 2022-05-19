<template>
  <footer>
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
    <div class="footer-bottom">
      <button class="footer-btn">Sign-up now!</button>
      <div class="social"></div>
    </div>
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
    width: 200px;
    margin-left: 200px;
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
@media screen and (max-width: 880px) {
  .footer-logo {
    display: none;
  }
}

.footer-bottom {
  height: 70px;
  background-color: #1c1c1c;
  display: flex;
  flex-wrap: wrap;
  & .footer-btn {
    height: 50%;
    width: 100px;
    margin-left: 200px;
    margin-top: 20px;
    font-size: 70%;
    background-color: #1c1c1c;
    border: solid 2px #0282f9;
    color: white;
    text-transform: uppercase;
  }
  & .social {
    height: 100%;
    width: 250px;
    margin-left: 30%;
    border: solid 1px white;//debug
  }
}
.col {
  margin-left: 40px;
}
</style>
