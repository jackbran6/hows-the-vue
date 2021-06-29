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
  </div>
</template>

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
  padding-right: 60px;
}
</style>
