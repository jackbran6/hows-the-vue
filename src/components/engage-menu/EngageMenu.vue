<template>
  <div class="card">
    <h3 class="button">+</h3>
    <h4 class="title">More ways to engage</h4>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'EngageMenu'
})
</script>

<style scoped>
  .card {
    align-items: center;
    align-self: center;
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 100%;
  }
  .button {
    font-size: 40px;
    padding-right: 10px;

  }
</style>
