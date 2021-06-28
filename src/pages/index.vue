<template>
  <div class="container">
    <div class="image">
      <TitleImage />
    </div>
    <div class="secondary-container">
      <MenuButton class="hamburger" />
      <ContactBox
        route="contact-us"
        title="Contact us"
        weekdays="12pm-11pm"
        weekend="3pm-11pm"
        contact="free call 0800 9428787"
      />
      <ContactBox
        route="chat"
        title="Chat online"
        weekdays="12pm-10pm"
        weekend="3pm-10pm"
        contact="whatsup.co.nz/chat"
      />
      <EngageMenu />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

import TitleImage from '@/components/title-image/TitleImage.vue'
import EngageMenu from '@/components/engage-menu/EngageMenu.vue'
import MenuButton from '@/components/menu-button/MenuButton.vue'
import ContactBox from '~/components/contact-boxes/ContactBox.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    TitleImage,
    ContactBox,
    EngageMenu,
    MenuButton
  },

  head: {
    title: 'Hello world!'
  }
})
</script>

<style scoped>
.container {
  display: grid;
  grid-template-columns: 3fr 2fr;
  margin: auto;
}

.hamburger {
  padding-right: 20px;
  padding-top: 40px;
  position: absolute;
  right: 0;
}
</style>
