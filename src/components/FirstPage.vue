<template>
  <div class="container">
    <div class="box-container">
      <div class="single-box" v-for="i in pageNumber" :key="i"></div>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  data() {
    return {
      pageNumber: 3,
    };
  },
};
</script>
<style lang="css">
.container {
  width: 100%;
  height: 100%;
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow-y: scroll;
}

.box-container {
  margin-top: 20vh;
  width: 65%;
  height: 100%;
  background: blue;
  display: flex;
  flex-wrap: wrap;
}

.single-box {
  width: 100%;
  max-height: 35%;
  background-color: white;
  border: 1px solid black;
}
</style>
