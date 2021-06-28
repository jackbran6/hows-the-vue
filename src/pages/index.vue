<template>
  <div class="container">
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
        <LinkBox
          route="contact-us"
          title="All our conversations are fully confidential"
          content="So don't worry you can talk to us about anything, we won't judge you and you won't get in trouble"
          route-title="Read more"
        />
        <TextBox
          content="We're here for all children and teenagers in Aotearoa."
        />
      </div>

      <ImageContent
        title="Talk to us about anything - it's free"
        content=" We're trained counsellors and are happy to help you with whatever you
      need. We can listen or give adivce. We're here for everything that's on
      your mind no matter how big or small."
      />
    </div>
    <div class="third-container">
      <TextBoxContent
        title="You can ask to speak with a man or woman counsellor"
        content="If you have spoken with a counselor before you can even ask to speak to the same person if you want to!"
        row="true"
      />
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
import TextBoxContent from '~/components/text-box/TextBoxContent.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    TitleImage,
    ContactBox,
    EngageMenu,
    MenuButton,
    LinkBox,
    ImageContent,
    TextBox,
    TextBoxContent
  }
})
</script>

<style scoped>
.container {
  margin: auto;
  width: 80vw;
}
.first-container {
  display: grid;
  grid-template-columns: 3fr 2fr;
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
