<template>
  <div class="container">
    <div class="section-one">
      <h3 class="call">Call us</h3>
      <h3 class="chat">Chat now</h3>
    </div>
    <div class="menu-bar">
      <ul class="menu">
        <li class="menu-item">About Us</li>
        <li class="menu-item">Our Promise</li>
        <li class="menu-item">Our Partners</li>
        <li class="menu-item">Our Toolkit</li>
      </ul>
    </div>
    <div class="footer">
      <div class="barnardos">
        <p class="barnardos-text">
          0800 What's Up is part of the Barnardos whānau
        </p>
        <p class="charities-text">
          Charities Commision Number: CC21844 - Registration details on the
          Charities Commission website
        </p>
      </div>
      <Button title="Donate" subtitle="On barnardos.co.nz" />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Button from '@/components/button/Button.vue'
export default Vue.extend({
  name: 'Footer',
  components: {
    Button
  }
})
</script>

<style lang="scss" scoped>
.container {
  background-color: #f4f4f4;
  padding: 200px 100px;
}
.section-one {
  display: flex;
  flex-direction: row;
}
.call {
  color: #045a55;
  font-size: 2rem;
  padding-right: 100px;
}
.chat {
  color: #045a55;
  font-size: 2rem;
}
.menu {
  display: flex;
  flex-direction: row;
}
.menu-item {
  color: #045a55;
  font-weight: 600;
  padding-right: 60px;
  padding-top: 50px;
}
.footer {
  align-items: flex-end;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-top: 300px;
}
.barnardos-text {
  color: #045a55;
  font-weight: 600;
}
.charities-text {
  color: #045a55;
  font-weight: 600;
}
</style>
