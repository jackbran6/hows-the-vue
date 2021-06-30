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
    <div class="fourth-container">
      <div class="resources">
        <TitleWithContent
          title="Resources"
          content="If you don't feel like talking right now, find helpful tips below."
        />
        <div class="resource-links">
          <ResourceLink title="Kids" tereo="Tamariki" />
          <ResourceLink title="Family" tereo="Rangatahi" />
          <ResourceLink title="Family" tereo="Whānau" />
        </div>
        <Title title="Follow us" class="follow-title" />
        <div class="follow-content">
          <FollowContent />
          <FollowContent />
          <FollowContent />
          <FollowContent />
        </div>
        <FollowLinks />
      </div>
    </div>
    <div class="fifth-container">
      <Barnardos />
    </div>
    <div class="sixth-container">
      <Partners />
      <Promote />
    </div>
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

import LinkBox from '@/components/link-box/LinkBox.vue'
import ImageContent from '@/components/image-content/ImageContent.vue'
import TextBox from '@/components/text-box/TextBox.vue'
import Title from '@/components/title/Title.vue'
import ResourceLink from '@/components/resource-links/ResourceLink.vue'
import TitleWithContent from '@/components/title/TitleWithContent.vue'
import FollowLinks from '@/components/follow-links/FollowLinks.vue'
import Barnardos from '@/components/barnardos/Barnardos.vue'
import Partners from '@/components/partners/Partners.vue'
import Promote from '@/components/promote/Promote.vue'

import TextBoxContent from '~/components/text-box/TextBoxHorizontal.vue'
import HomePageTop from '~/components/page-sections/homepage-top/HomePageTop.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    LinkBox,
    ImageContent,
    TextBox,
    TextBoxContent,
    Title,
    ResourceLink,
    TitleWithContent,
    FollowLinks,
    Barnardos,
    Partners,
    Promote,
    HomePageTop
  }
})
</script>

<style scoped>
.container {
  margin: auto;
}
.first-container {
  display: grid;
  grid-template-columns: 3fr 2fr;
}

.second-container {
  display: grid;
  grid-template-columns: 2fr 3fr;
  margin: auto;
}
.sixth-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  margin: auto;
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
.resource-links {
  column-gap: 50px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  justify-content: center;
}
.follow-content {
  column-gap: 50px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  justify-content: center;
}
.follow-title {
  padding-top: 50px;
}
.resources {
  background: #fff;
  padding: 50px;
}
</style>
