<template>
  <div class="lading-image-container">
    <div class="elements">
      <img
        src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Gull_portrait_ca_usa.jpg"
        alt=""
      />
      <div class="image-text">aaa</div>
    </div>
  </div>
</template>
<script lang="ts">
export default {};
</script>
<style lang="css">
.lading-image-container {
  width: 100%;
  /*height: 100%;*/
  display: flex;
  justify-content: center;
}
.elements {
  width: 70%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.elements > img {
  height: 80vh;
  max-width: 100%;
}
.image-text {
  width: 100%;
  height: 20vh;
  background-color: red;
}

@media screen and (max-width: 800px) {
  .elements {
    width: 100%;
  }
}
</style>
