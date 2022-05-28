<template>
  <div class="container">
    <div class="box-container">
      <div class="single-box" v-for="(info, i) in infos" :key="i">
        <div class="paragraph">
          <div class="title">
            {{ info.title }}
          </div>
          <div class="text">
            {{ info.text }}
          </div>
        </div>
        <div class="image">
          <img :src="info.image" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
export default {
  data() {
    return {
      infos: [
        {
          title: "titolo2",
          text: "macchine elettriche storia funzioni caratteristiche vantaggi/svantaggi ecc",
          image: "src",
        },
        {
          title: "titolo3",
          text: "stazioni di ricarica funzionamento costi velocita caratteristiche  ",
          image: "src",
        },
      ],
    };
  },
};
</script>
<style lang="css">
.container {
  width: 100%;
  height: 80%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.box-container {
  width: 70%;
  min-height: 100%;
  background: blue;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: stretch;
}

.single-box {
  width: 100%;
  background-color: white;
  border: 1px solid black;
  display: flex;
  justify-content: center;
  align-items: center;
}
.single-box:nth-child(even) > .paragraph {
  order: 2;
}

.paragraph {
  width: 67%;
  height: 100%;
  background-color: green;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.title{
  height: 20%;
}
.text{
  height: 80%;
}

.image {
  width: 33%;
  height: 100%;
  background-color: yellow;
}

@media screen and (max-width: 800px){
  .box-container{
    width: 100%;
  }
}
</style>
