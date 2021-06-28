<template>
  <div class="menu-container">
    <div class="line"></div>
    <div class="line"></div>
    <div class="line"></div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'MenuButton'
})
</script>

<style scoped>
.line {
  background: #fff;
  height: 5px;
  margin-bottom: 5px;
  width: 60px;
}
</style>
