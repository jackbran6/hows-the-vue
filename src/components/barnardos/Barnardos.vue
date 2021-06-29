<template>
  <div class="content-container">
    <p class="barnardos-text">0800 What's Up is part of the Barnardos whānau</p>
    <h3 class="call-to-action">
      In 2020 we answered over 19,707 calls and web chats.
    </h3>
    <div class="donate-container">
      <p class="donate-statement">Help us continue with our work</p>
      <Button title="Donate" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Button from '@/components/button/Button.vue'
export default Vue.extend({
  name: 'Barnardos',
  components: {
    Button
  }
})
</script>

<style scoped>
.content-container {
  background: #009639;
  display: flex;
  flex-direction: column;
  padding: 50px;
}
.barnardos-text {
  color: #fff;
}
.call-to-action {
  color: #fff;
  font-size: 3rem;
  line-height: 3.2rem;
  padding-top: 100px;
}
.donate-container {
  align-items: center;
  display: flex;
  flex-direction: row;
  padding-top: 100px;
}
.donate-statement {
  color: #fff;
  font-size: 1rem;
  font-weight: 600;
  padding-right: 30px;
}
.donate-text {
  color: #fff;
  font-size: 1rem;
  font-weight: 600;
}
.button {
  background-color: #ed8b00;
  border-radius: 3px;
  padding: 15px 30px;
}
</style>
