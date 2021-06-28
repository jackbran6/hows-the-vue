<template>
  <div class="content-container">
    <h3 class="title">
      {{ content }}
    </h3>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'TextBox',
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
  background: #fab6a6;
  justify-content: center;
  padding: 100px 50px;
}
</style>
