<template>
  <div class="">
    <div class="first-container">
      <MenuButton class="hamburger" />
      <div class="image">
        <TitleImage />
      </div>
      <div class="secondary-container">
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
          :check="true"
        />
        <EngageMenu />
      </div>
    </div>
    <div class="second-container">
      <div class="secondary-container">
        <LinkBox route="contact-us" />
        <TextBox />
      </div>

      <ImageContent />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

import TitleImage from '@/components/title-image/TitleImage.vue'
import EngageMenu from '@/components/engage-menu/EngageMenu.vue'
import MenuButton from '@/components/menu-button/MenuButton.vue'
import ContactBox from '@/components/contact-boxes/ContactBox.vue'
import LinkBox from '@/components/link-box/LinkBox.vue'
import ImageContent from '@/components/image-content/ImageContent.vue'
import TextBox from '@/components/text-box/TextBox.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    TitleImage,
    ContactBox,
    EngageMenu,
    MenuButton,
    LinkBox,
    ImageContent,
    TextBox
  },

  head: {
    title: 'Hello world!'
  }
})
</script>

<style scoped>
.first-container {
  display: grid;
  grid-template-columns: 3fr 2fr;
  margin: auto;
  width: 80vw;
}

.second-container {
  display: grid;
  grid-template-columns: 2fr 3fr;
  margin: auto;
  width: 80vw;
}

.hamburger {
  justify-self: flex-end;
  padding-right: 20px;
  padding-top: 40px;
  position: absolute;
}
.secondary-container {
  height: 100%;
}
</style>
