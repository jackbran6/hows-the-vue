<template>
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
</template>

<script lang="ts">
import Vue from 'vue'

import TitleWithContent from '@/components/title/TitleWithContent.vue'
import ResourceLink from '@/components/resource-links/ResourceLink.vue'
import FollowContent from '@/components/follow-us/FollowContent.vue'
import Title from '@/components/title/Title.vue'
import FollowLinks from '@/components/follow-links/FollowLinks.vue'
export default Vue.extend({
  name: 'ResourceSection',
  components: {
    TitleWithContent,
    ResourceLink,
    FollowContent,
    Title,
    FollowLinks
  }
})
</script>

<style scoped>
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
