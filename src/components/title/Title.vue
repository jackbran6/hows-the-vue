<template>
  <div class="content-container">
    <h3 class="title">
      {{ title }}
    </h3>
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
