<template>
<div class="container">
  <div class="image">
    <TitleImage/>
  </div>
  <div class="secondary-container">
    <ContactBox route="contact-us" title="Contact us" weekdays="12pm-11pm" weekend="3pm-11pm" contact="free call 0800 9428787"/>
    <ContactBox route="chat" title="Chat online" weekdays="12pm-10pm" weekend="3pm-10pm" contact="whatsup.co.nz/chat"/>
    <EngageMenu/>
  </div>
</div>

</template>
<script lang="ts">
import Vue from 'vue'

import TitleImage from '@/components/title-image/TitleImage.vue'
import EngageMenu from '@/components/engage-menu/EngageMenu.vue'
import ContactBox from '~/components/contact-boxes/ContactBox.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    TitleImage,
    ContactBox,
    EngageMenu
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
margin: auto;
width: 80vw;
}
.image {
  background-color: rgb(253, 181, 193);
  display: flex;
  flex-grow: 5;
}
.secondary-container {
  background-color: rgb(233, 167, 233);
  flex-direction: column;
  flex-grow: 3;
}
</style>
