<template>
  <div class="navbar">
    <div v-for="page in pages" :key="page">
      <div class="inner-class">
        <a href="" class="link"> {{ page }} </a> 
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      pages: ["Home", "Mappe"],
    };
  },
};
</script>
<style>
.navbar {
  width: 100%;
  height: 10vh;
  
  background-color: red;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.inner-class {

}
.link{
  text-decoration: none;
  color: white;
}
</style>
