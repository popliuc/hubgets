<template>
  <div id="app">
    <HeaderLogo class="header-logo" />
    <br />
    <HeaderDescription />
    <div class="registration-body">
      <div class="empty-cell"></div>
      <Register />
      <RegistrationInfo class="registration-info" />
      <div class="empty-cell"></div>
    </div>
    <Footer />
  </div>
</template>

<script>
import HeaderLogo from "./components/HeaderLogo.vue";
import HeaderDescription from "./components/HeaderDescription.vue";
import Register from "./components/Register.vue";
import RegistrationInfo from "./components/RegistrationInfo.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "app",
  components: {
    HeaderLogo,
    HeaderDescription,
    Register,
    RegistrationInfo,
    Footer
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0px;
}
.header-logo {
  margin-top: 10px;
}
.registration-body {
  display: grid;
  grid-template-columns: 15% 35% 30% 20%;
  align-items: center;
  background-color: whitesmoke;
  padding-bottom: 10%;
}

.registration-info {
  padding-left: 30px;
}

@media screen and (max-width: 900px) {
  .registration-body {
    display: grid;
    grid-template-columns: 100%;
    align-items: center;
    background-color: whitesmoke;
    padding-bottom: 2%;
  }
  .empty-cell {
    display: none;
  }
}
</style>
