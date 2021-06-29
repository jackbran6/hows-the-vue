<template>
  <div class="content-container">
    <h3 class="title">
      {{ title }}
    </h3>
    <p class="content">
      {{ content }}
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Title',
  props: {
    title: {
      type: String,
      default: 'Default title'
    },
    content: {
      type: String,
      default: 'This is default content'
    }
  }
})
</script>

<style scoped>
.title {
  color: #06968f;
  font-size: 4rem;
}
h3 {
  margin: 0;
}
p {
  margin: 0;
}
.content {
  padding-bottom: 50px;
}
</style>
