<template>
  <div class="content-container">
    <h3 class="title">{{ title }}</h3>
    <p class="content">
      {{ content }}
    </p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'ImageContent',
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
.content-container {
  background: #c5e8e8;
  justify-content: center;
  padding: 100px 50px;
}
</style>
