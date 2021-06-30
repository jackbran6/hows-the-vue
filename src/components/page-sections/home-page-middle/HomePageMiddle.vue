<template>
  <div class="container">
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
        row
      />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

import TextBox from '@/components/text-box/TextBox.vue'
import TextBoxContent from '@/components/text-box/TextBoxHorizontal.vue'
import ImageContent from '@/components/image-content/ImageContent.vue'
import LinkBox from '@/components/link-box/LinkBox.vue'
export default Vue.extend({
  name: 'HomePageMiddle',
  components: {
    TextBox,
    TextBoxContent,
    ImageContent,
    LinkBox
  }
})
</script>

<style scoped>
.second-container {
  display: grid;
  grid-template-columns: 2fr 3fr;
  margin: auto;
}
</style>
