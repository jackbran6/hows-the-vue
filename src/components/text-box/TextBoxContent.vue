<template>
  <div class="content-container" :class="{ secondary: row }">
    <h3 class="title">
      {{ title }}
    </h3>
    <p class="content">{{ content }}</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'TextBoxContent',
  props: {
    content: {
      type: String,
      default: 'Default title'
    },
    title: {
      type: String,
      default: 'This is default content'
    },
    row: {
      type: Boolean,
      default: false
    }
  }
})
</script>

<style scoped>
.content-container {
  background: #ffe8b3;
  justify-content: center;
  padding: 100px 50px;
}
.secondary {
  display: grid;
  grid-template-columns: 2fr 3fr;
}
</style>
