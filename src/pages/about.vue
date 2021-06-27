<template>
  <Intro>
    <h3 class="title">About</h3>
    <p class="content">This is some content</p>
  </Intro>
</template>

<script lang="ts">
import Vue from 'vue'
import Intro from '@/components/intro/Intro.vue'
export default Vue.extend({
  name: 'About',
  components: {
    Intro,
  }
})
</script>

