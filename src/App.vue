<template>
  <div class="vue-container">
    <NavBar></NavBar>
    <FirstPage></FirstPage>
  </div>
</template>
<script lang="ts">
import FirstPage from "./components/FirstPage.vue";
import NavBar from "./components/NavBar.vue";

export default {
  components: {
    FirstPage,
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
  background-color: white;
}
.vue-container {
  height: 100vh;
}
</style>
