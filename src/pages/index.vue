<template>
<div class="container">
  <div class="image">
    <TitleImage/>
  </div>
  <div class="secondary-container">
    <ContactBox title="Contact Us" weekdays="12pm-11pm" weekend="3pm-11pm" contact="free call 0800 9428787"/>
    <ContactBox title="Chat Online" weekdays="12pm-10pm" weekend="3pm-10pm" contact="whatsup.co.nz/chat"/>
  </div>
</div>

</template>
<script lang="ts">
import Vue from 'vue'

import TitleImage from '@/components/title-image/TitleImage.vue'
import ContactBox from '@/components/contact-boxes/ContactUs.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    TitleImage,
    ContactBox
  },

  head: {
    title: 'Hello world!'
  }
})
</script>

<style scoped>
.container {
display: flex;
flex-direction: row;
height: 100vh;
margin: auto;
width: 80vw;
}
.image {
  display: flex;
  flex-grow: 5;
}
.secondary-container {
  flex-direction: column;
  flex-grow: 3;
}
.section-one {
  background-color: rgb(221, 236, 236);
  flex-grow: 2;
}
.section-two{
  background-color: rgb(201, 59, 59);
  flex-grow: 2;
}
.section-three {
  background-color: rgb(223, 179, 122);
  flex-grow: 2;
}
</style>
