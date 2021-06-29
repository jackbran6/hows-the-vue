<template>
  <div class="">
    <button class="button">
      <p class="title-text">{{ title }}</p>
      <p class="subtitle-text">{{ subtitle }}</p>
    </button>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'Button',
  props: {
    title: {
      type: String,
      default: 'Donate'
    },
    subtitle: {
      type: String,
      default: ''
    }
  }
})
</script>

<style scoped>
.button {
  background-color: #ed8b00;
  border-radius: 3px;
  padding: 15px 30px;
}
.title-text {
  color: #fff;
  font-size: 1rem;
  font-weight: 600;
}
.subtitle-text {
  color: #fff;
  font-size: 1rem;
  font-weight: 400;
}
</style>
