<template>
  <div class="dummy-image">
    <img class="image" src="@/assets/images/prismic-logo.png" alt="sample image">
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'TitleImage'
})
</script>

<style scoped>
.dummy-image{
  background-color: rgb(250, 202, 210);
  height: 600px;
  width: 600px
}
.image {
  height: 100%;
  width: 100%;
}
</style>
