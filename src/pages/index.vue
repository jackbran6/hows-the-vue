<template>
  <div class="container">
    <HomePageTop />
    <HomePageMiddle />
    <ResourceSection />
    <div class="barnardos-container">
      <Barnardos />
    </div>
    <PartnerPromotions />
  </div>
</template>
<script lang="ts">
import Vue from 'vue'

import Barnardos from '@/components/barnardos/Barnardos.vue'
import HomePageMiddle from '@/components/page-sections/home-page-middle/HomePageMiddle.vue'
import ResourceSection from '@/components/page-sections/resource-section/ResourceSection.vue'
import PartnerPromotions from '@/components/page-sections/partner-promotions-section/PartnerPromotions.vue'
import HomePageTop from '~/components/page-sections/homepage-top/HomePageTop.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    ResourceSection,
    Barnardos,
    HomePageTop,
    HomePageMiddle,
    PartnerPromotions
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
