<template>
  <div class="content-container">
    <h3 class="title">All our conversations are fully confidential</h3>
    <p class="content">
      So don't worry you can talk to us about anything, we won't judge you and
      won't get you in trouble
    </p>
    <nuxt-link :to="route">Read More</nuxt-link>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'LinkBox',
  props: {
    route: {
      type: String,
      default: ''
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
</style>
