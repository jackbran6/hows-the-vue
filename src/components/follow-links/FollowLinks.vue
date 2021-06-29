<template>
  <div class="content-container">
    <a href="https://www.facebook.com/0800Whatsup/" class="facebook">
      <p>Facebook</p>
    </a>
    <a href="https://www.instagram.com/0800whatsup/?hl=en" class="instagram">
      <p>Instagram</p>
    </a>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  name: 'TextBox'
})
</script>

<style scoped>
.content-container {
  display: flex;
  flex-direction: row;
  padding-top: 15px;
}
.facebook {
  border-bottom: 2.5px solid currentColor;
  color: #0d5f5b;
  margin-right: 20px;
  text-decoration: none;
}
.instagram {
  border-bottom: 2.5px solid currentColor;
  color: #0d5f5b;
  text-decoration: none;
}
</style>
