<template>
  <div class="">
    <div class="content-container"></div>
    <h3 class="title">{{ title }}</h3>
    <p class="te-reo">{{ tereo }}</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ResourceLink',
  props: {
    title: {
      type: String,
      default: 'Default Title'
    },
    tereo: {
      type: String,
      default: 'This is default content'
    }
  }
})
</script>

<style scoped>
.content-container {
  background: #fab6a6;
  height: 20rem;
  padding: 20px;
}
.title {
  color: #045a55;
  font-size: 2rem;
  padding-top: 10px;
}
.te-reo {
  color: #045a55;
}
h3 {
  margin: 0;
}
</style>
