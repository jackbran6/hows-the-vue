<template>
<div class="container">
  <div class="image"></div>
  <div class="secondary-container">
    <div class="section-one"></div>
    <div class="section-two"></div>
    <div class="section-three"></div>
  </div>
</div>

</template>
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home',
  components: {

  },

  head: {
    title: 'Hello world!'
  }
})
</script>

<style scoped>
.container {
background-color: rgb(247, 188, 197);
display: flex;
flex-direction: row;
height: 100vh;
margin: auto;
width: 80vw;
}
.image {
  background-color: rgb(248, 232, 210);
  display: flex;
  flex-grow: 5;
}
.secondary-container {
  flex-direction: column;
  flex-grow: 3;
}
.section-one {
  background-color: rgb(221, 236, 236);
  flex-grow: 2;
}
.section-two{
  background-color: rgb(201, 59, 59);
  flex-grow: 2;
}
.section-three {
  background-color: rgb(223, 179, 122);
  flex-grow: 2;
}
</style>
