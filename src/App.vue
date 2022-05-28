<template>
  <div class="vue-container">
    <NavBar></NavBar>
    <LandingPage></LandingPage>
    <FirstPage></FirstPage>
  </div>
</template>
<script lang="ts">
import FirstPage from "./components/FirstPage.vue";
import LandingPage from "./components/LandingPage.vue";
import NavBar from "./components/NavBar.vue";

export default {
  components: {
    FirstPage,
    LandingPage,
    NavBar,
  },
};
</script>
<style lang="css">
* {
  box-sizing: border-box;
}
body {
  margin: 0;
  background-color: rgb(0, 0, 0);
}
.vue-container {
  height: 120vh;
}
</style>
