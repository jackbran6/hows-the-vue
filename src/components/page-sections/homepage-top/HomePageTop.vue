<template>
  <div class="first-container">
    <div class="image">
      <TitleImage />
    </div>
    <div>
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
        check
      />
      <EngageMenu />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

import ContactBox from '@/components/contact-boxes/ContactBox.vue'
import TitleImage from '@/components/title-image/TitleImage.vue'
import EngageMenu from '@/components/engage-menu/EngageMenu.vue'

export default Vue.extend({
  name: 'HomePageTop',
  components: {
    ContactBox,
    TitleImage,
    EngageMenu
  }
})
</script>

<style scoped>
.first-container {
  display: grid;
  grid-template-columns: 3fr 2fr;
}
</style>
