<template>
  <div class="content-container">
    <h3 class="title">{{ title }}</h3>
    <p class="content">
      {{ content }}
    </p>
    <nuxt-link :to="route">{{ routeTitle }}</nuxt-link>
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
    },
    title: {
      type: String,
      default: 'Default title'
    },
    content: {
      type: String,
      default: 'This is default content'
    },
    routeTitle: {
      type: String,
      default: 'Default route title'
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
