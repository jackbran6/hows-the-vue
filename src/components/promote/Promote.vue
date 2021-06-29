<template>
  <div class="content-container">
    <div class="image"></div>
    <p class="promote">Promote 0800 What's Up in your school or community</p>
    <p class="learn">Learn more about our toolkit</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Promote',
  props: {
    content: {
      type: String,
      default: 'This is default content'
    }
  }
})
</script>

<style scoped>
.content-container {
  background: #c5e8e8;
  justify-content: center;
  padding: 50px;
}
.image {
  background-color: #fff;
  height: 450px;
  width: 75%;
}
.promote {
  font-size: 2rem;
  font-weight: 600;
  padding-top: 20px;
}
.learn {
  padding-top: 100px;
}
</style>
