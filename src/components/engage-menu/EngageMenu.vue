<template>
  <div class="card">
    <h3 class="button">+</h3>
    <h4 class="title">More ways you can engage</h4>
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
  background-color: #ed8b00;
  display: flex;
  flex-direction: row;
  justify-content: center;
  width: 100%;
}
.button {
  font-size: 40px;
  padding-right: 10px;
}
.title {
  align-self: center;
}
</style>
